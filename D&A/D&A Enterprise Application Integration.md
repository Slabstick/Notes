- EAI und ESB (Enterprise Service Bus)
- Alternative Lösung zu Vaults/Warehouse/Lake
- Im Gegensatz zur Warehouses nahezu Realtime (Neartime) Verarbeitung

## EAI 

- Planung, Methoden und Software um Anwendungen in einem Unternehmen zu integrieren
- ESB ist eine Methode, die notwendige Kommunikation technisch zu ermöglichen

## ESB

- Schlimmster Fall: 1:1 (Spaghetti)

### N:m Vermindungen: Kanonisches Datenformat als Zentrale Anlaufstelle (Knotenpunkt) für alle Daten

- Einheitliches Format für einen Nachrichtentyp, der von allen verstanden wird

### Prozessloser ESB - dummer ESB, smarte Clients

- Wenn Kunde Logik möchte baut man Adapter außerhalb des ESBs

### Praxis

- Routing - Camel - Nachrichtenübertragung
- Broker - ActiveMQ, Kafka, Artemis, ... - Nachrichten entgegen nehmen und im ESB verteilen
- Transformation - Java, Simple (Camel), ... - Umwandlung
- Runtime - Apache Karaf - Umgebung in der Camel-Routen permanent laufen
- Management - Custom Made

#### Beispiel

Camel-Route läuft in der Runtime, ließt Dateien aus einem Ordner ein und sendet sie an einen Kafka Broker. -> Talend ESB (Was ganz anderes als Talend DI) liefert Routing (Camel), Transformation (Java), Runtime (Karaf) und Management (Console)

