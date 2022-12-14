Falls ihr eure Antworten nochmal mit den richtigen vergleichen wollt, hab ich euch mal eine kleine Musterlösung zusammengeschrieben. Hoffe es hilft. ![🙂](https://statics.teams.cdn.office.net/evergreen-assets/personal-expressions/v2/assets/emoticons/smile/default/30_f.png?v=v81)



## **1. Was ist die Zahl 42 im Binärsystem?**   

Die Zahl 42 setzt sich aus folgenden Zweierpotenzen zusammen:

-   2^5 = 32
-   2^3 = 8
-   2^1 = 2  

Die Exponenten 5, 3, 1 entsprechen den Stellen in der Binärzahl, die „1“ sind:

Stelle:    5 4 3 2 1 0  
Binärzahl: 1 0 1 0 1 0

Die richtige Antwort ist also 101010

  

## **2. Was ist die Binärzahl 1001 im Dezimalsystem?**   

 In der Frage ging es um das reine Binärsystem, **ohne** Einerkom plement / Vorzeichenbit / etc. Erst muss herausgefunden werden, welche Stellen der Binärzahl „1“ ergeben.  

Stelle:    3 2 1 0   
Binärzahl: 1 0 0 1   

In unserem Fall ist das die „nullte“ und dritte Stelle. Dann rechnet man die Zweierpotenzen für diese Stellen aus und summiert sie auf: 2^3 + 2^0 = 8 + 1 = 9

  

## **3. Was ergibt die Rechnung „101 + 11“ im Binärsystem?**  

In Binär kann man genau so wie im Dezimalsystem Zahlen addieren. Dabei fängt man von rechts an:  

101 + 11 -> 1 + 1 ergibt 10, wir notieren uns die 0 als rechteste Zahl und merken uns 1 als Übertrag   

101 + 11 -> 0 + 1 ergibt 1. Aus der letzten Rechnung haben wir aber noch den Übertrag 1, den wir hier mit addieren müssen. Es ergibt sich 1+1 = 10. Wie vorher notieren wir 0 und merken uns 1 als Übertrag.   

101 + 11 -> Es gibt nur noch die Stelle 1, die aber wieder mit dem Übertrag aus der vorherigen Zeile verrechnet werden muss. Es ergibt wieder 10.   

Die notierten Zahlen schreibt man zusammen zu 1000

  

## **4. Welche Ziffern gibt es im Hexadezimalsystem?**   

Es gibt folgende Ziffern: 0 1 2 3 4 5 6 7 8 9 A B C D E F.  

Wichtig ist, dass die 0 nicht vergessen wird. :)

  

## **5. Was ergibt die Rechnung „EF + 3“ im Hexadezimalsystem?**  

Hier war der Gedanke, dass ihr nicht „richtig“ rechnen sollt, sondern lediglich drei mal „hochzählt“, also:   

EF + 1 = F0  

 F0 + 1 = F1  

 F1 + 1 = F2

  

## **6. Wie wird das Einerkomplement gebildet?**   

Das Einerkomplement wird für negative Zahlen gebildet, indem alle Bits invertiert werden. Das erste Bit gibt dadurch das Vorzeichen an: 0 bedeutet positiv, 1 bedeutet negativ.

  

## **8. Was ist die Einerkomplementdarstellung (mit 8 Bits) für die Dezimalzahl „-9“?**   

Erst wird die 9 in eine Binärzahl umgewandelt. Sie setzt sich aus den Zweierpotenzen 2^3 = 8 und 2^0 = 1 zusammen. Es ergibt sich die Binärzahl 1001. Sobald wir mit Vorzeichenbit, Einerkomplement oder Zweierkomplement arbeiten, müssen wir auf die Anzahl an Bits achten, die uns zur Verfügung stehen. In der Fragestellung sind es 8 Bits. Dementsprechend füllen wir unsere Binärzahl links mit 0en auf: 00001001.  
Da wir -9 darstellen wollen, invertieren wir nochmal jedes Bit: 11110110 Damit sind wir fertig.  

## **9. Was ist die Zweierkomplementdarstellung (mit 8 Bits) für die Dezimalzahl „-3“?**  

Die Zahl 3 ergibt sich aus den Zweierpotenzen 2^1 = 2 und 2^0 = 1. Es ergibt sich die Binärzahl 11. Auch hier arbeiten wir wieder mit 8 verfügbaren Bits, wodurch sich 00000011 ergibt. Dann bilden wir das Einerkomplement, indem wir jedes Bit invertieren: 11111100.  
Anschließend gelangen wir zum Zweierkomplement, indem wir noch 1 addieren: 11111100 + 1 = 11111101  

## **10. Was ist der Vorteil der Zweierkomplementdarstellung?**   

Das Zweierkomplement vereinfacht die Subtraktion: Statt eine Zahl zu subtrahieren, kann man die Zahl zu einer negativen-Zahl umrechnen und addieren. Zudem wird die 0 eindeutig dargestellt und dadurch keine Zahl „verschwendet“.