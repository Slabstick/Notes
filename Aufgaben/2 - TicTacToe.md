#HTTP #TCP/IP #Postman #Websockets #ServerSockets

# Webkommunikation

- Client Server Architektur
- Server
	- Client bekommt eine Kopie der Seite, wenn Client Anfrage schickt
- Kommunikation über TCP/IP
	- Protokoll, das den Standard vorgibt über den kommuniziert wird
- HTTP
	- Definiert wie Daten in der Kommunikation aussehen
- Websockets
	- Einmaliges Öffnen der Verbindung
	- Läuft auch über TCP
	- Danach bleibt sie bestehen, bis sie getrennt wird
	- Z.B. genutzt für Chats
	- Kein Polling (aktives Nachfragen nach Antworten)

## Aufgabe 1
- Create a ServerSocket
	- ServerSocket at a dedicated port
	- Open a connection
	- Retrieve any message from a client (Postman)
	- Respond with "Hello World"
		- Needs to be in the HTTP Format, otherwise Postman will reject it
- All processes should be logged
	- Logger should print to the console in different colors, based on severity
		- info, warn, error, error with exception, fatal, fatal with exception
		- All methods should support the String.format(...) notation

## Postman
- Kann Requests schicken und sich die Responses angucken

## Aufgabe 2

#### 1.1 Extract information from request (Header)  
+ Parse Request Header  
+ Extract all Headerfields  
#### 1.2 Extract information from request (params + body)  
+ parse request parameter  
+ parse request body
+ Send the request body back as response
### 1.3 Only process request if auth header is attached  
+ Check for auth header  
+ extract username and passwort from header
+ https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/403
+ https://developer.mozilla.org/en-US/docs/Web/HTTP/Status
### 1.4 Encrypt (& decrypt) passwords
- https://www.baeldung.com/sha-256-hashing-java


## Aufgabe 3

