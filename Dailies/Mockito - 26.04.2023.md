``` java
package Angi; 
import org.junit.jupiter.api.AfterEach; 
import org.junit.jupiter.api.BeforeEach; 
import org.junit.jupiter.api.Test; 
import org.mockito.Mockito; 
import java.io.ByteArrayOutputStream; 
import java.io.PrintStream; 
import java.util.Scanner; 
import static org.junit.jupiter.api.Assertions.assertEquals; 
import static org.mockito.Mockito.*; 

class UserInputMockingTest { 
	private final UserInput userInput = new UserInput(); 
	private final PrintStream standardOut = System.out; 
	private final ByteArrayOutputStream outputStreamCaptor = new ByteArrayOutputStream(); 

	@BeforeEach 
	void setUp() { 
		System.setOut(new PrintStream(outputStreamCaptor)); 
	} 
	
	@AfterEach 
	void tearDown() { 
	System.setOut(standardOut); 
	} 
	
	@Test 
	void testGetPositionFromPlayer_withCorrectInputOnFirstTry_expectPositionAndVerifyNoFieldPrinting() { 
		Scanner scanner = mockScanner("A7"); 
		GameBoard gameBoard = mockGameboard("A7"); 
		String positionFromPlayer = userInput.getPositionFromPlayer(scanner, gameBoard); 
		assertEquals("A7", positionFromPlayer); 
		verify(gameBoard, Mockito.never()).printCurrentPlayField(); 
	} 
	
	@Test 
	void testGetPositionFromPlayer_withCorrectInputOnSecondTry_expectPositionAndVerifyOneFieldPrinting() { 
		Scanner scanner = mockScanner("asdasdasdasd", "a8"); 
		GameBoard gameBoard = mockGameboard("A8"); 
		String positionFromPlayer = userInput.getPositionFromPlayer(scanner, gameBoard); 
		assertEquals("A8", positionFromPlayer); 
		verify(gameBoard).printCurrentPlayField(); 
		assertEquals("Invalid input! Try again.\n", outputStreamCaptor.toString()); 
	} 
	
	@Test 
	void testGetPositionFromPlayer_withCellUnavailableAndCorrectInputOnSecondTry_expectPositionAndVerifyOneFieldPrinting() { 
		Scanner scanner = mockScanner("asdasdasdasd", "a8"); 
		GameBoard gameBoard = mockGameboard("A8"); 
		when(gameBoard.isUserInputValid("Asdasdasdasd")) .thenReturn(true); 
		String positionFromPlayer = userInput.getPositionFromPlayer(scanner, gameBoard); 
		assertEquals("A8", positionFromPlayer); 
		verify(gameBoard).printCurrentPlayField(); 
		assertEquals("Position unavailable. Choose another position.\n", outputStreamCaptor.toString()); 
	} 
	
	private GameBoard mockGameboard(String validInput) { 
		GameBoard gameBoard = mock(GameBoard.class); 
		when(gameBoard.isUserInputValid(validInput)) 
			.thenReturn(true); 
		when(gameBoard.isCellAvailable(validInput)) 
			.thenReturn(true); return gameBoard; 
	} 
	
	private Scanner mockScanner(String nextLine, String... nextLines) { 
		Scanner scanner = mock(Scanner.class); 
		when(scanner.nextLine()) 
			.thenReturn(nextLine, nextLines); 
		return scanner; 
	} 
}
```

