
# Einleitung
## Projektumfeld

Die QuinScape GmbH ist ein deutscher IT-Dienstleister, welcher bereits seit über 20 Jahren als Spezialist in den Themenbereichen Data & Analytics und Software Engineering aktiv ist. Mit Hilfe der Vielzahl an Partnern und den mittlerweile über 200 MitarbeiterInnen, die in dem Hauptsitz Dortmund, sowie dem Nebenstandort Hannover tätig sind, realisiert das Unternehmen individuelle Lösungen für die anspruchsvollen Bedürfnisse seiner KundInnen. Seit 2021 agiert die QuinScape GmbH außerdem als Gründungsunternehmen der Dataciders GmbH (ehemals QuinScape Group), die mittlerweile acht weitere Unternehmen der IT-Branche beinhaltet. Die Dataciders GmbH beschäftigt insgesamt über 500 Personen aus mehr als 15 Nationen.


## Ausgangssituation

Viele Menschen haben Schwierigkeiten, ihre Ernährungsgewohnheiten zu überwachen und gesundheitliche Ziele zu erreichen, da sie oft nicht über die notwendigen Informationen oder Werkzeuge verfügen, um ihre Nahrungsaufnahme effektiv zu verfolgen. Besonders die Wahl von kalorienarmen Nahrungsmitteln fällt vielen Menschen schwer, da sie im Supermarkt durch Werbung, Marketing und offizielle Qualitätssiegel und Verpackungsaufdrucke verwirrt und oft auch getäuscht werden.

## Projektbeschreibung

Bei dem vorgestellten Projekt handelt es sich um ein eigenständiges Projekt, welches intern in der Software Engineering Abteilung der QuinScape GmbH entwickelt wird. Die Anforderungen an das Projekt werden von Herrn Florian Hillmann gestellt, welcher als Kunde auftritt.

In diesem Projekt soll eine webbasierte Anwendung entwickelt werden, die NutzerInnen ermöglicht, ihre tägliche Nahrungsaufnahme zu verfolgen und detaillierte Informationen über die Nährwerte ihrer Mahlzeiten zu erhalten. Ziel ist es, das Bewusstsein und das Verständnis der NutzerInnen für ihre Ernährung zu verbessern und sie bei der Erreichung ihrer gesundheitlichen und fitnessbezogenen Ziele zu unterstützen.

## Projektziel

Das Hauptziel dieses Projektes ist die Entwicklung einer intuitiven und benutzerfreundlichen Anwendung, die es NutzerInnen nicht nur ermöglicht, ihre tägliche Kalorienaufnahme einfach zu protokollieren und zu überwachen, sondern auch einen Einblick in ihre Makronährstoffverteilung (Proteine, Kohlenhydrate, Fette) gibt. Diese Funktionalität ist essentiell, um nicht nur Gewichtsverlustziele zu unterstützen, sondern auch spezifische Fitness- und Gesundheitsziele, wie den Muskelaufbau oder die Verbesserung der allgemeinen Körperzusammensetzung, zu erreichen.

Die Anwendung bietet eine Datenbank mit Nahrungsmitteln, die detaillierte Informationen zu Kalorien und Makronährstoffen enthält. NutzerInnen können durch diese Datenbank nach bereits gespeicherten Nahrungsmitteln suchen, um ihre täglichen Mahlzeiten zusammenzustellen, oder eigene Nahrungsmittel hinzufügen, falls diese nicht vorhanden sind. Jedes Nahrungsmittel kann mit der entsprechenden Menge zum persönlichen Ernährungstagebuch hinzugefügt werden, welches automatisch die Summe der konsumierten Kalorien und Makronährstoffe für den Tag berechnet.

Die Benutzeroberfläche ist darauf ausgelegt, den Ablauf so einfach wie möglich zu gestalten. NutzerInnen können direkt von der Startseite aus auf die Funktionen zum Hinzufügen von Mahlzeiten, Durchsuchen der Nahrungsmitteldatenbank und Anzeigen ihres Ernährungstagebuchs zugreifen. Das Tagebuch präsentiert eine klare und verständliche Zusammenfassung der täglichen Nahrungsaufnahme. Ob es darum geht, Gewicht zu verlieren, Muskelmasse aufzubauen oder einfach eine ausgewogenere Ernährung zu pflegen, die App bietet die Werkzeuge, die NutzerInnen benötigen, um informierte Entscheidungen über ihre Ernährung zu treffen und ihre Gesundheits- und Fitnessziele zu erreichen.

## Projektschnittstellen

### Personenschnittstellen

Die Anforderungen des Projekts stammen von einem Mitarbeiter der QuinScape GmbH, Herrn Florian Hillmann, der hier als Kunde auftritt. Folglich ist Herr Hillmann auch derjenige, dem das Projektergebnis präsentiert wird und an welchen die Übergabe stattfinden wird. Das langfristige Ziel ist es die Applikation für Smartphones verfügbar zu machen, zunächst aber soll nur ein funktionierender Prototyp erstellt werden, der einem ausgewählten Kreis von NutzerInnen zur Verfügung gestellt wird.

### Technische Schnittstellen

Die einzige technische Schnittstelle findet sich hier innerhalb der Applikation selbst zwischen dem Back- und Frontend in Form einer RESTful API. Weitere Schnittstellen werden erst in zukünftigen Versionen der Applikation nötig, wenn z.B. eine Nutzerdatenbank implementiert und auf öffentliche Datenbanken von Drittanbietern zugegriffen wird. Dies ist im Rahmen dieses Projekts vorerst aber nicht vorgesehen.

## Projektabgrenzung

### Unterschiede zu Projektantrag

Im Großen und Ganzen wurde das Projekt dem Antrag entsprechend durchgeführt. Einzige Abweichung findet sich darin, dass es keine dedizierte Startseite gibt, sondern NutzerInnen sofort den Log, den zie zuletzt bearbeitet haben oder den Log des aktuellen Datums öffnen. Dies ist mit einer verbesserten User Experience zu erklären, da eine dedizierte Startseite hier nicht mehr zeitgemäß wäre. Sollten in Zukunft noch weitere Funktionen hinzukommen, könnte man über die Implementierung eines so genannten Dashboards nachdenken.

## Technologien

### Java

Für das Spring Boot Backend wurde die Programmiersprache Java in der Version 21 verwendet, da diese die vom Unternehmen meist genutzte Programmiersprache ist.
Java selbst ist eine objektorientierte Programmiersprache, welche sowohl Elemente einer Compiler- als auch einer Interpretersprache hat, da deren Quellcode vor der Ausführung in Bytecode kompiliert wird, welcher dank der Java Virtual Machine auf beliebigen Endgeräten ausführbar ist.
Das macht sie plattformunabhängiger als Compilersprachen wie z.B. C++.

### JavaScript/TypeScript

Für die Frontend-Entwicklung wurde die Programmiersprache TypeScript verwendet, die auf JavaScript basiert. TypeScript ist eine von Microsoft entwickelte, statisch typisierte Superset-Sprache von JavaScript, die zusätzliche Typ-Sicherheit und modernere Sprachmerkmale bietet. Durch die Verwendung von TypeScript können Entwickler Fehler frühzeitig im Entwicklungsprozess erkennen und beheben, was zu stabilerem und wartbarerem Code führt. Der TypeScript-Code wird in JavaScript transpiliert, welches von allen modernen Webbrowsern unterstützt wird. JavaScript ist eine dynamisch typisierte, interpretierte Sprache, die hauptsächlich zur Entwicklung interaktiver Webanwendungen verwendet wird. Beide Sprachen sind plattformunabhängig und können auf verschiedenen Geräten und Umgebungen ausgeführt werden.

### Spring Boot

Für die Entwicklung des Backends wurde das Spring Boot Framework verwendet. Spring Boot ist ein Open-Source-Framework, das auf dem weitverbreiteten Spring Framework basiert und speziell dafür entwickelt wurde, das Erstellen von Production-Ready-Anwendungen mit minimalem Konfigurationsaufwand zu erleichtern. Es bietet zahlreiche vorkonfigurierte Starter-Pakete und automatisch konfigurierte, eingebettete Webserver wie Tomcat und Jetty, um den Einstieg erheblich zu vereinfachen. Mit Spring Boot können Entwickler RESTful Webservices, Microservices und moderne Cloud-Native-Anwendungen entwickeln, die leicht skalierbar und wartbar sind. Darüber hinaus ermöglicht das Framework durch sein umfangreiches Ecosystem und Unterstützung für diverse Datenbank- und Messaging-Integrationen die reibungslose Entwicklung komplexer Unternehmensanwendungen.

### SQLite3

Für die Datenverwaltung wurde die Datenbank-Engine SQLite3 verwendet. SQLite3 ist eine serverlose, selbst in die Anwendung eingebettete relationale Datenbank, die sich durch ihre geringen Anforderungen und unkomplizierte Integration auszeichnet. Im Gegensatz zu schweren, serverbasierten Datenbanksystemen wie MySQL oder PostgreSQL benötigt SQLite3 keine separate Serverinstallation und Konfiguration. Die gesamte Datenbank wird in einer einzigen Datei gespeichert, was sie ideal für lokale Anwendungsdaten und embedded Systeme macht. Zudem bietet SQLite3 eine vollständige SQL-Unterstützung, hohe Zuverlässigkeit und schnelle Lese- und Schreibvorgänge. Diese Eigenschaften machen SQLite3 besonders geeignet für Anwendungen mit geringem bis mittlerem Datenaufkommen, Entwicklungs- und Testumgebungen sowie mobile oder Desktop-Applikationen.

### React

Für die Entwicklung des Frontends wurde die JavaScript-Bibliothek React verwendet. React wurde von Meta (ehemals Facebook) entwickelt und ist heute eine der am häufigsten verwendeten Bibliotheken für die Erstellung moderner, dynamischer Benutzeroberflächen. Durch das Prinzip der komponentenbasierten Architektur ermöglicht React die Wiederverwendung von UI-Komponenten, was die Entwicklung und Wartung von Anwendungen vereinfacht. React verwendet ein Virtuelles DOM (Document Object Model), das effiziente Updates und Renderings von Komponenten ermöglicht, wodurch die Performance und Reaktionsschnelligkeit der Anwendung verbessert werden. Mit seiner starken Community und einer Vielzahl an unterstützenden Bibliotheken und Tools, wie React Router für die Navigation und Redux für das State-Management, ist React eine leistungsfähige Wahl für die Erstellung skalierbarer und wartbarer Webanwendungen.

### TailwindCSS

Für das Styling der Anwendung wurde das Utility-First CSS-Framework Tailwind CSS verwendet. TailwindCSS ermöglicht ein schnelles und effizientes Erstellen von benutzerdefinierten Designs direkt im HTML-Markup, indem es eine Vielzahl von vorgefertigten CSS-Klassen bereitstellt, die einzeln oder in Kombination genutzt werden können. Im Gegensatz zu traditionellen CSS-Frameworks bietet Tailwind CSS keinen vordefinierten Designstil, sondern gibt EntwicklerInnen die Flexibilität, ihr eigenes Designsystem zu erstellen und gleichzeitig konsistente und wartbare Stile sicherzustellen. Durch die Verwendung von Tailwind CSS können spezifische Designs ohne die Notwendigkeit, benutzerdefiniertes CSS zu schreiben, schnell prototypisiert und umgesetzt werden. Dies führt zu einer sauberen, minimalen Stylesheet-Datei und einer besseren Performance der Anwendung. Zudem ermöglicht das aufeinander abgestimmte Ecosystem von Tailwind CSS, einschließlich Plugins und Integrationen, eine nahtlose Anpassung und Erweiterung der Funktionalität.

### Shadcn/ui

Für die Benutzeroberfläche wurde das Shadcn/ui-Framework eingesetzt. Shadcn/ui ist ein modernes UI-Framework, das sich durch seine hohe Anpassungsfähigkeit und Benutzerfreundlichkeit auszeichnet. Es bietet eine Vielzahl von vorgefertigten Komponenten, die leicht in bestehende Projekte integriert werden können, und ermöglicht es EntwicklerInnen, schnell und effizient ansprechende Benutzeroberflächen zu erstellen. Shadcn/ui unterstützt eine komponentenbasierte Architektur und bietet umfangreiche Möglichkeiten zur Anpassung der Komponentenstile, wodurch eine konsistente und individuell gestaltbare UI gewährleistet wird. Durch die Nutzung dieses Frameworks können Entwicklungszeiten reduziert und die Wartbarkeit der Anwendung verbessert werden. Mit Shadcn/ui kann die Produktivität gesteigert werden, während gleichzeitig eine hohe Qualität und Benutzerfreundlichkeit der Benutzeroberfläche sichergestellt wird.

### NPM

Neben den Hauptbibliotheken und Frameworks wurden auch verschiedene kleinere Pakete aus dem Node Package Manager (NPM) Repository integriert, um spezifische Funktionalitäten zu ergänzen und die Entwicklung zu erleichtern. NPM ist das weltweit größte Software-Registry, die es EntwicklerInnen ermöglicht, Open-Source-Pakete einfach zu suchen, zu installieren und zu verwenden. Die Auswahl an Paketen bietet eine breite Palette von Lösungen für Probleme wie etwa Form-Handling, Validierung, Zustandmanagement und Animationen. Durch die Nutzung dieser Pakete konnte die Entwicklungszeit verkürzt und die Codequalität verbessert werden. Die modularen und gut dokumentierten NPM-Pakete tragen zur Flexibilität und Erweiterbarkeit der Anwendung bei, indem sie es ermöglichen, standardisierte und geprüfte Lösungen zu integrieren, ohne von Grund auf neu schreiben zu müssen.

### Git

Für das Versionsmanagement und die Zusammenarbeit im Entwicklungsteam wurde Git als Versionskontrollsystem verwendet. Git ist ein verteiltes Versionskontrollsystem, das eine vollständige Historie aller Änderungen an der Codebasis ermöglicht und somit die Nachverfolgbarkeit und Wiederherstellbarkeit früherer Versionen sicherstellt. Es unterstützt eine effiziente und kollaborative Arbeitsweise, indem es EntwicklerInnen ermöglicht, gleichzeitig an verschiedenen Features und Bugfixes zu arbeiten, ohne sich gegenseitig zu behindern. Das Branching-Modell von Git erleichtert den Workflow erheblich, da Änderungen isoliert vorgenommen und nur dann in den Hauptzweig integriert werden, wenn sie stabil und getestet sind. Darüber hinaus wurde Bitbucket genutzt, um Code-Repositories zentral zu hosten und die später evtl. noch relevante Integration von CI/CD-Pipelines zu unterstützen. Bitbucket erleichtert nicht nur das Code-Review und das Management von Pull Requests, sondern bietet auch Tools zur Automatisierung von Tests


# Ressourcen- und Ablaufplanung

## Personalplanung

## Sachmittelplanung

Folgende Hardware und Ressourcen wurden zur Verfügung gestellt:

- MacBook Pro (2021)
- Tastatur
- Maus
- Dockingstation
- Monitor
- Backup Festplatte

Folgende Software wurde zur Verfügung gestellt:

- MacOS Sonoma Version 14.5
- IntelliJ IDEA Ultimate Edition Version 2024.1.1
- Jira
- BitBucket
- Microsoft Teams
- Microsoft Outlook
- Postman

Ein Büro wurde nicht genutzt, da zu 100% remote gearbeitet wurde.

## Projektphasen

Zur Durchführung des Projekts wurde folgender Zeitplan erstellt:

| Phase                     | Aufgabe                           | Zeit (Std.) |
| ------------------------- | --------------------------------- | ----------- |
| **Analysephase**          |                                   | **6**       |
|                           | Ist-Analyse                       | 1           |
|                           | Soll-Konzept                      | 5           |
| **Planungsphase**         |                                   | **4**       |
|                           | Terminplanung                     | 1           |
|                           | Sachmittelplanung                 | 1           |
|                           | Kostenplanung                     | 1           |
|                           | Personalplanung                   | 1           |
| **Entwurfsphase**         |                                   | **20**      |
|                           | Design des Backends               | 8           |
|                           | Design des Frontends              | 8           |
|                           | Entwurf der Datenbankstrukturen   | 2           |
|                           | Entwurf der API Endpunkte         | 2           |
| **Implementierungsphase** |                                   | **30**      |
|                           | Implementierung des Backends      | 16          |
|                           | Implementierung der API Endpunkte | 2           |
|                           | Anbindung an Datenbank            | 2           |
|                           | Implementierung der Webseite      | 10          |
| **Testphase**             |                                   | **8**       |
|                           | Erstellen von Tests               | 8           |
| **Schlussphase**          |                                   | **12**      |
|                           | Projektdokumentation              | 8           |
|                           | Anwenderdokumentation             | 2           |
|                           | Bereitstellung                    | 2           |


## Terminplanung

Die Durchführung des Projektes verläuft parallel zum Tagesgeschäft der QuinScape GmbH vom 18.03.2024 bis zum 27.05.2024 (Kalenderwochen 12 - 22). Die folgende Tabelle veranschaulicht die Terminplanung:

| Phase                 | Zeit/h | KW 14 | 15  | 16  | 17  | 18  | 19  | 20  | 21  | 22  |
| --------------------- | ------ | ----- | --- | --- | --- | --- | --- | --- | --- | --- |
| Analysephase          | 6      | 6     |     |     |     |     |     |     |     |     |
| Planungsphase         | 4      | 4     |     |     |     |     |     |     |     |     |
| Entwurfsphase         | 20     |       | 10  | 10  |     |     |     |     |     |     |
| Implementierungsphase | 30     |       |     |     | 13  | 7   | 5   | 5   |     |     |
| Testphase             | 8      |       |     |     | 1   | 2   | 2   | 3   |     |     |
| Schlussphase          | 12     |       |     |     |     |     |     | 4   | 4   | 4   |
| Gesamt                | 80     |       |     |     |     |     |     |     |     |     |


## Kostenplanung

### Projektkosten

Die Kosten für das Projekt setzen sich aus Ressourcen- und Personalkosten zusammen.
Daten der zu veranschlagenden Kosten für Auzubildende, EntwicklerInnen sowie die Nutzung von Ressourcen wurden von der Verwaltung der QuinScape GmbH zur Verfügung gestellt. So betragen die Kosten für Auszubildende 9,50€/h und 60€/h für EntwicklerInnen. Die Kosten zur Bereitstellung der Ressourcen belaufen sich bei Auszubildenden pauschal auf einen Betrag von 15€/h und müssen zusätzlich auf den oben genannten Betrag addiert werden. Die pauschalen Ressourcenkosten, welche für EntwicklerInnen anfallen, sind im genannten Betrag jedoch bereits inbegriffen. Die Gesamtkosten bzw. Kostenaufstellung des Projektes sind in der folgenden Tabelle zu sehen:

| Vorgang            | Zeit in h | Kosten pro Stunde in € | Kosten in € |
| ------------------ | --------- | ---------------------- | ----------- |
| Entwicklungskosten | 80        | 9,50 + 15 = 24,50      | 1960        |
| Black-Box-Test     | 2         | 60                     | 120         |
| Abnahmetest        | 6         | 60                     | 360         |
| Übergabe           | 2         | 60                     | 120         |
| Gesamt             |           |                        | 2560        |


# Durchführung und Auftragsbearbeitung

Zur Durchführung des Projekts wurde ein modernes und agiles Projektmanagementmodell genutzt. Auch wenn das Projekt nur einen Entwickler hat, wurde sich an dem SCRUM Vorgehensmodell orientiert. Durch das iterative Durchlaufen der Projektphasen und die stetige Absprache mit dem Product Owner Herrn Hillmann, war eine agile und flexible Anpassung der Anforderungen des Projekts jederzeit möglich. Außerdem konnten unbekannte, neu aufgetretene Probleme mit Schnittstellen außerhalb des Einflussbereiches gelöst werden, ohne den Ablauf des Vorgehensmodells zu verändern.
![[scrum-framework-9.29.23.png]]
## Analysephase

### IST-Analyse
Derzeit gibt es eine Vielzahl von Anwendungen auf dem Markt, die NutzerInnen dabei helfen, ihre Nahrungsaufnahme zu verfolgen und Makronährstoffe zu berechnen. Viele dieser Apps bieten Funktionen wie die Möglichkeit, Lebensmittel durch Barcodes zu scannen, umfangreiche Nahrungsmitteldatenbanken, und die Integration mit Fitness-Trackern. Allerdings gibt es noch immer Lücken und Schwächen in den bestehenden Lösungen. NutzerInnen berichten häufig über unzureichende Lebensmittel-Datenbanken, umständliche Benutzeroberflächen und fehlende Anpassungsmöglichkeiten für individuelle Ernährungspläne. Auch bei der Unterstützung konkreter Fitnessziele wie Gewichtsreduktion oder Muskelaufbau sehen viele AnwenderInnen Verbesserungspotential. Daher besteht ein klarer Bedarf an einer intuitiven, benutzerfreundlichen App, die präzise Nahrungsmittelinformationen bietet und sich nahtlos in den Alltag der NutzerInnen integrieren lässt, um ihre Fitnessziele effektiver zu erreichen.

### SOLL-Analyse

#### Anforderungen

##### 1. Benutzerfreundlichkeit

- Die App muss für Smartphone-Bildschirme optimiert sein, um eine nutzerfreundliche Bedienung zu gewährleisten.

- Beim Start der App soll  NutzerInnen automatisch das Log des Tages angezeigt werden, das sie sich als letztes angeschaut haben.

##### 2. Hauptfunktionen

- Die App soll zwei Hauptfunktionen bieten: Logs und die Nahrungsmitteldatenbank.

- Von überall in der App sollen NutzerInnen sofort Zugriff auf diese beiden Hauptfunktionen sowie einen Knopf haben, mit dem sie automatisch ein Nahrungsmittel in die Datenbank speichern können.

##### 3. Nahrungsmitteldatenbank

- NutzerInnen sollen in der Datenbank Nahrungsmittel hinzufügen, bearbeiten oder löschen können.

- Aus der Datenbank soll ein Nahrungsmittel direkt zu einem Log hinzugefügt werden können.

##### 4. Logs

- Im Log sollen NutzerInnen hinzugefügte Nahrungsmittel bearbeiten oder löschen können.

- NutzerInnen sollen im Log zu einem anderen Datum wechseln können, um vergangene Einträge anzusehen oder zu ändern.

- In jedem Log soll eine Berechnung der Kalorienanzahl und Makronährstoffe in Summe dargestellt werden.

### Zieldefinition

Die zu entwickelnde App soll folgende Ziele erreichen: 

1. **Benutzerfreundlichkeit und Intuition** 
- Die App soll eine benutzerfreundliche und intuitive Möglichkeit bieten, die tägliche Nahrungsaufnahme zu verfolgen und Makronährstoffe zu berechnen. 

2. **Optimierung für Smartphones** 
- Im Vergleich zu existierenden Lösungen soll die App durch ihre Optimierung für Smartphone-Bildschirme überzeugen. 

3. **Einfache Fortführung der Aufzeichnungen** 
- Beim Start präsentiert die App das zuletzt betrachtete Tageslog, um den NutzerInnen eine einfache Fortführung ihrer Aufzeichnungen zu ermöglichen. 

4. **Zugriff auf Hauptfunktionen** 
- Zwei Hauptfunktionen stehen im Vordergrund: die Nahrungsmitteldatenbank und die Logs. 
- Beide Funktionen sollen von jeder Ansicht aus sofort erreichbar sein. 

5. **Zentrale Schaltfläche für schnelle Aktionen** 
- Eine zentrale Schaltfläche ermöglicht das schnelle Hinzufügen neuer Nahrungsmittel zur Datenbank, die dann wiederum direkt zu den Logs hinzugefügt, bearbeitet oder gelöscht werden können. 

6. **Flexible Verwaltung der Log-Einträge** 
- Innerhalb der Logs können NutzerInnen ihre Einträge flexibel verwalten und zwischen unterschiedlichen Datumseinträgen wechseln. 

Diese Kernfunktionen sollen eine effektive Unterstützung bei der Verfolgung der täglichen Nahrungsaufnahme und der Zielsetzung für Makronährstoffe bieten.

## Planungsphase

Diese wurde bereits in Kapitel 2 ausführlich dargestellt und kann dort eingesehen werden.

## Entwurfsphase

### Entwurfsmuster MVC - Model View Controller

#### Verständnis des MVC Entwurfsmusters

Das MVC (Model-View-Controller) Entwurfsmuster ist ein bewährtes Softwaredesign-Paradigma, das weit verbreitet in der Softwareentwicklung eingesetzt wird, um Anwendungen strukturiert und wartbar zu gestalten. Es teilt eine Anwendung in drei wesentliche Komponenten auf:

1. **Model (Modell)**:
    
    - Das Modell repräsentiert die Daten und die Geschäftslogik der Anwendung. Es ist verantwortlich für das Speichern, Verarbeiten und Verwalten von Daten. Das Modell stellt sicher, dass die Daten konsistent und validiert sind, und kann zu Datenbanken oder anderen Speichersystemen gehören.
    - Beispiel: In einer Nahrungsmittel-Tracking-App könnte das Modell Informationen über Nahrungsmittel, Nährwerte und Tageslogs enthalten.
2. **View (Ansicht)**:
    
    - Die Ansicht ist für die Darstellung der Daten an den Benutzer zuständig. Sie zeigt die Informationen aus dem Modell in einer für die BenutzerInnen verständlichen und ansprechenden Form an. Die Ansicht enthält keine Geschäftslogik, sondern stellt nur das Darstellungslogik bereit.
    - Beispiel: Die Ansicht in unserer App wäre die Benutzeroberfläche, die den NutzerInnen ermöglicht, Nahrungsmittel zu sehen, hinzuzufügen oder zu bearbeiten.
3. **Controller (Steuerung)**:
    
    - Der Controller fungiert als Vermittler zwischen Modell und Ansicht. Er verarbeitet Benutzerinteraktionen, Aktualisierungen und Eingaben, aktualisiert das Modell entsprechend und leitet diese Änderungen an die Ansicht weiter. Der Controller enthält die Anwendungslogik und ist für die Bearbeitung von Eingaben verantwortlich.
    - Beispiel: Wenn NutzerInnen ein neues Nahrungsmittel hinzufügen, empfängt der Controller diese Aktion, erstellt das entsprechende Datenmodell und aktualisiert die Ansicht, um das neue Nahrungsmittel anzuzeigen.

#### Vorteile des MVC-Entwurfsmusters

Das MVC-Entwurfsmuster bietet mehrere Vorteile, die die Softwareentwicklung erleichtern und die Qualität des Codes verbessern:

- **Trennung der Anliegen**: Durch die Trennung des Codes in Modell, Ansicht und Controller werden die Verantwortlichkeiten klar definiert und der Code bleibt übersichtlich und wartbar. Dies erleichtert es EntwicklerInnen, an verschiedenen Teilen der Anwendung zu arbeiten, ohne sich gegenseitig zu behindern.
    
- **Wiederverwendbarkeit**: Komponenten des Modells und der Ansicht können unabhängig vom Rest der Anwendung wiederverwendet werden. Dies spart Entwicklungszeit und reduziert Redundanzen.
    
- **Einfachere Wartung und Erweiterbarkeit**: Da die Geschäftslogik (Modell), die Darstellung (Ansicht) und die Eingabelogik (Controller) getrennt sind, ist es einfacher, Änderungen vorzunehmen und Erweiterungen zur Anwendung hinzuzufügen, ohne dass die gesamte Anwendung umgeschrieben werden muss.
    

#### Anwendung in unserer App

In der Entwicklung unserer Nahrungsmittel-Tracking-App wird das MVC-Entwurfsmuster durchgängig angewendet:

- Das **Model** kümmert sich um die Verwaltung und Speicherung der Nahrungsmitteldaten und Logs. Dieses finden wir in der SQLite3 Datenbank wieder und ist einer von zwei Bausteinen des Backends.
- Die **View** sorgt dafür, dass die Benutzeroberfläche ansprechend und benutzerfreundlich ist. Diese wird in Form des Frontends implementiert werden.
- Der **Controller** übernimmt die Eingaben der NutzerInnen, führt die entsprechende Logik aus und aktualisiert sowohl das Modell als auch die Ansicht, um den NutzerInnen eine konsistente und reaktionsschnelle Benutzererfahrung zu bieten. Dieser ist der zweite Teil des Backends und wird im Java/Spring Boot Code manifestiert.

Durch die Implementierung des MVC-Entwurfsmusters wird sichergestellt, dass unsere App strukturiert, leicht wartbar und erweiterbar bleibt.

### Backend

Die Entwicklung des Backends der App basiert auf Technologien und folgt bewährten Methoden, welche bei QuinScape auch im Tagesgeschäft zum Einsatz kommen. Im Zentrum dieser Entwicklung steht Spring Boot, ein leistungsstarkes Framework, das die Erstellung von robusten und produktionsreifen Java-Anwendungen erleichtert. Mit Spring Boot lassen sich die wesentlichen Komponenten des Backends schnell und effizient implementieren.

Die Kommunikation zwischen dem Frontend und dem Backend erfolgt über eine RESTful API. Diese API nutzt die HTTP-Methoden (GET, POST, PUT, DELETE) zur Durchführung von CRUD-Operationen (Create, Read, Update, Delete). Diese Methode stellt sicher, dass Daten auf eine konsistente und zuverlässige Weise abgerufen und manipuliert werden können.

Für die Datenspeicherung wird SQLite3 als eingebettete Datenbank verwendet. SQLite3 ist eine leichtgewichtige Datenbank, die sich hervorragend für mobile Anwendungen eignet und eine einfache Integration und Verwaltung der gespeicherten Daten bietet.

Das Backend wird mit Java 21 entwickelt, einer modernen Version der Java-Programmiersprache, die zahlreiche neue Features und Verbesserungen bietet. Maven wird als Build- und Management-Tool verwendet. Dieses erleichtert die Verwaltung der Projektabhängigkeiten und automatisiert viele Aspekte des Entwicklungsprozesses, was zu einer effizienteren und konsistenteren Entwicklung führt. Sämtliche für das Projekt erforderlichen Abhängigkeiten werden in einer XML-Datei (`pom.xml`) definiert. Diese Datei beschreibt alle notwendigen Bibliotheken und Frameworks, die für die reibungslose Funktion des Backends erforderlich sind.

#### Vier Schichten Struktur

Um das MVC Entwurfsmuster noch feiner zu strukturieren, wird der Controller, also der Java-Teil, als solcher noch einmal in vier Layer unterteilt. Dem Datenmodell am nächsten liegt die Repository-Schicht, welche den direkten Zugriff auf die Datenbank und die Verwaltung der Daten ermöglicht. Diese Schicht enthält die Codes für CRUD-Operationen (Create, Read, Update, Delete) und stellt sicher, dass die Datenbankabfragen effizient und korrekt ausgeführt werden.

Über der Repository-Schicht befindet sich die Service-Schicht. Diese Schicht dient als Mittler zwischen der Repository-Schicht und der Controller-Schicht und enthält die Geschäftslogik der Anwendung. Sie stellt sicher, dass die Daten auf eine sinnvolle und konsistente Art und Weise verarbeitet werden. Die Service-Schicht ruft Methoden aus der Repository-Schicht auf und führt die erforderlichen Operationen wie Validierungen oder Datenmanipulationen durch.

Die Controller-Schicht selbst nimmt die HTTP-Anfragen von der Benutzeroberfläche entgegen und gibt die entsprechenden Antworten zurück. Sie ist für die Verarbeitung der Benutzerinteraktionen verantwortlich und leitet die Anfragen an die Service-Schicht weiter. Die Controller-Schicht stellt somit sicher, dass die richtigen Datenmodelle und -methoden verwendet werden, um die Anfragen zu erfüllen.

Schließlich gibt es noch die Model-Schicht, welche die Domänenobjekte oder Entitätsklassen der Anwendung definiert. Diese Schicht repräsentiert die Geschäftsobjekte, die von der Anwendung verwendet werden, und bildet die zugrundeliegende Struktur der Daten ab. Die Model-Schicht stellt sicher, dass die Daten klar strukturiert und in einem konsistenten Format vorliegen.

#### Model-Schicht

Um eine Übersicht darüber zu gewinnen, welche Entitäten benötigt werden, bietet sich ein Entity-Relation-Modell der Datenbank an. Daraus lässt sich ableiten, dass drei Tabellen erforderlich sind. Zwei dieser Tabellen sind für die im Entwurf erarbeiteten Hauptfunktionen des Programms vorgesehen (Log und Nahrungsmittel, hier „nutrition_log“ und „food_item“). Eine weitere Tabelle ordnet die Nahrungsmittel als abgeleitete Entität den jeweiligen Logs zu. Da Nahrungsmittel mehrfach pro Log hinzugefügt werden können, muss diese Entität („food_item_entry“) ihren eigenen Primärschlüssel haben und darf diesen nicht aus den anderen beiden Tabellen kombinieren.

So ergibt sich das folgende Datenbankmodell:

![[SCR-20240522-oktd-2.png]]

Nach kurzer Beobachtung fällt auf, dass „food_item“ und „nutrition_log“ die gleichen Attributsbezeichnungen verwenden. Diese lassen sich daher für Java in eine eigene Klasse extrahieren. Für die Model-Schicht in Java ergibt sich somit die folgende Struktur:

![[SCR-20240522-oqbl-2.png]]

Damit wäre das Datenmodell vollständig modelliert. In Verbindung mit den Zielsetzungen lassen sich nun die weiteren Schichten des Spring Boot Backends definieren.

#### Repository-Schicht

Die Repository-Schicht spielt eine zentrale Rolle in der Datenzugriffsschicht einer Anwendung. In unserem Projekt wird diese Schicht mithilfe von **Spring Data JPA** implementiert.

**Spring Data JPA** ist ein Teil von Spring Data, einem Projekt innerhalb des Spring Frameworks, das darauf abzielt, die Implementierung von Datenzugriffsschichten für verschiedene persistente Speicher zu vereinfachen. Spring Data JPA bietet eine abstrakte und einfach zu nutzende Schnittstelle für die Interaktion mit relationalen Datenbanken, indem es die Java Persistence API (JPA) nutzt.

**Spring Data JPA** reduziert den Boilerplate-Code für die Datenzugriffsschicht erheblich und ermöglicht es den EntwicklerInnen, sich mehr auf die Geschäftslogik zu konzentrieren. Es bietet eine Reihe von Vorteilen, darunter:

- **Automatische Generierung von CRUD-Methoden**: Spring Data JPA generiert automatisch grundlegende CRUD-Methoden (Create, Read, Update, Delete) für Ihre Entitäten, sodass Sie sich nicht um die Implementierung dieser Methoden kümmern müssen.
- **Abfrage-Derivation**: Sie können benutzerdefinierte Abfragen einfach durch das Definieren von Methoden entsprechend benannter Muster in Ihren Repository-Interfaces erstellen.
- **Paging und Sortierung**: Spring Data JPA unterstützt Paging und Sortierungen auf einfache und intuitive Weise.

##### Erstellung von Repositories in Java

Die Implementierung eines Repositories in Spring Data JPA beginnt mit der Definition eines Interfaces, das von einem der von Spring bereitgestellten Repository-Interfaces wie "JpaRepository", "CrudRepository" oder "PagingAndSortingRepository" erbt. 

##### Vereinfachung von CRUD-Operationen mit SQL

Dank Spring Data JPA werden die CRUD-Operationen stark vereinfacht. Hier sind einige grundlegende Methoden, die out-of-the-box verfügbar sind:

- **save()**: Speichert eine Entität in der Datenbank.
- **findById()**: Findet eine Entität anhand ihres Primärschlüssels.
- **findAll()**: Findet alle Entitäten in der Datenbank.
- **deleteById()**: Löscht eine Entität anhand ihres Primärschlüssels.

##### Repository Methoden

Die meisten Methoden der Repository-Schicht sind bereits durch Spring Data JPA vorgegeben und müssen nur in besonderen Fällen explizit definiert werden. Für unseren Anwendungsfall ergibt sich folgendes Bild:

![[Repo-Layer.png]]

Wie im Diagramm ersichtlich, müssen lediglich das „FoodItemRepository“ zwei und das „NutritionLogRepository“ eine spezifische Methode definieren. Alle anderen CRUD-Operationen sind so häufig und standardisiert, dass sie von Spring Data JPA automatisch bereitgestellt werden und nicht gesondert definiert werden müssen.

###### Methode findByDate
Da jeder Log-Eintrag nur einmal pro Datum existieren kann, kann die Suche nach spezifischen Logs vereinfacht werden, indem statt der Suche nach der ID eine Methode erstellt wird, die einen Log-Eintrag anhand des Datums findet. Dies kann bestimmte Funktionen im Frontend erheblich vereinfachen.

###### Methode findByNameIgnoreCase
Diese Methode ist eine Erweiterung der implizit bereitgestellten „findByName“-Methode. Da Nahrungsmittel mit demselben Namen in der Datenbank nur einmal existieren sollen, wird diese Methode benötigt, um keine Unterscheidung zwischen Groß- und Kleinschreibung zu machen. Andernfalls wäre beispielsweise „Apfel“ ein anderes Objekt als „apfel“. Eine weitere Methode, „findByNameIgnoreCaseContaining“, gibt eine Liste von Objekten zurück, deren Namen das gesuchte Wort beinhalten, unabhängig von der Groß- oder Kleinschreibung.

#### Service-Schicht

Die Verwendung einer dedizierten Service-Schicht bietet mehrere Vorteile. Erstens ermöglicht sie die Kapselung der Geschäftslogik an einem zentralen Ort, was die Wartung und das Testen erheblich erleichtert. Zweitens fördert sie die Trennung der Verantwortlichkeiten: Durch die Trennung der Geschäftslogik von der Präsentations- und Datenzugriffsschicht sorgt sie für einen klaren und übersichtlichen Code. Darüber hinaus erhöht sie die Wiederverwendbarkeit, da Services von verschiedenen Controllern wiederverwendet werden können. Schließlich bieten Services eine einheitliche Schnittstelle für die Geschäftslogik, was die Flexibilität und Erweiterbarkeit der Anwendung verbessert.

Die Implementierung der Service-Schicht beginnt in Spring Boot mit der Definition von Service-Klassen, die in der Regel mit der Annotation "@Service" versehen werden. Diese Klassen enthalten Methoden, die die Geschäftslogik und die Verarbeitung von Daten implementieren. Ein normaler Service orchestriert die Interaktion mit der Repository-Schicht und stellt sicher, dass alle Geschäftsanforderungen erfüllt werden.

Für unsere Applikation ergeben sich daher folgende Klassen:

![[Service-Layer.png]]

Besonders auf zwei Arten von Methoden soll hier näher eingegangen werden: Zum einen die „upsert“-Methoden, zum anderen die „calculateNutrients“-Methode. Alle anderen Methoden sollten selbsterklärend benannt sein und keiner weiteren Erläuterung bedürfen.

###### Methoden upsertFoodItem & upsertNutritionLog

Eine **Upsert-Methode** im Backend kombiniert die Funktionen von **Update** und **Insert** in einer einzigen Operation. Das Wort „upsert“ ist ein Kofferwort aus den englischen Begriffen „update“ und „insert“. Eine Upsert-Methode überprüft, ob ein Datensatz in der Datenbank existiert. Wenn der Datensatz existiert, wird er aktualisiert (update). Wenn der Datensatz nicht existiert, wird ein neuer Datensatz erstellt und eingefügt (insert). Diese Methoden sind besonders nützlich, um unnötige separate Überprüfungen und Datenbankoperationen zu vermeiden.

Daraus ergibt sich, dass wir unsere API-Endpunkte übersichtlicher halten können, da wir für das Anlegen und das Aktualisieren eines Objekts nur einen Endpunkt benötigen und das Frontend nicht wissen muss, ob bereits ein Objekt existiert oder erst angelegt werden muss. Wollen wir beispielsweise ein Nahrungsmittel zu einem Log hinzufügen, das noch gar nicht existiert, rufen wir denselben Endpunkt auf, und das Backend legt dieses Log für uns an.

###### Methode calculateNutrients

Auch hier soll dem Frontend Arbeit abgenommen und Geschäftslogik in der Service-Schicht automatisiert werden. Diese Methode ist eine Helfermethode, die jedes Mal beim Abrufen eines Logs ausgeführt wird. So wird sichergestellt, dass die Summe aller Kalorien und Makronährstoffe auf dem neuesten Stand ist, sobald ein Log über den jeweiligen GET-Endpunkt abgerufen wird.

#### Controller-Schicht

Ein wesentlicher Aspekt der Controller-Schicht ist die Eingangsvalidierung. Bevor eine Anfrage zur Service-Schicht weitergeleitet wird, überprüft der Controller die eingehenden Daten auf Richtigkeit und Vollständigkeit. Dies dient zum einen dazu, Fehler frühzeitig zu erkennen und die Datenintegrität zu gewährleisten, und zum anderen, die Service- und Repositories-Schicht vor unnötiger Verarbeitung fehlerhafter Daten zu schützen.

Nachdem die Validierung abgeschlossen ist, leitet der Controller die Anfrage an die entsprechenden Service-Methoden weiter. Hier wird die Geschäftslogik angewendet und gegebenenfalls Daten aus der Repository-Schicht abgerufen oder gespeichert. Die Antwort der Service-Schicht wird dann vom Controller entgegengenommen und in ein Format umgewandelt, das für das Frontend verständlich und brauchbar ist – in unserem Fall im JSON Format, da unser Frontend in TypeScript/JavaScript geschrieben ist und daher nativ das JSON (JavaScript Object Notation) Format unterstützt.

Darüber hinaus ist der Controller auch dafür verantwortlich, geeignete HTTP-Statuscodes zurückzugeben, die den Ausgang der Anfrage widerspiegeln. Bei erfolgreicher Verarbeitung wird häufig der Statuscode 200 (OK) oder 201 (Created) verwendet, während bei Fehlern entsprechende Codes wie 400 (Bad Request) oder 404 (Not Found) gesendet werden.

In einer gut strukturierten Applikation ist die Controller-Schicht so gestaltet, dass sie nur minimale Logik enthält und hauptsächlich als Schnittstelle dient. Die eigentliche Geschäftslogik bleibt der Service-Schicht vorbehalten, um eine klare Trennung der Verantwortlichkeiten zu gewährleisten. Dies fördert die Wartbarkeit und Testbarkeit der Anwendung und erlaubt eine einfache Erweiterung der Endpunkte bei zukünftigen Anforderungen.

Beachten wir diese Anforderungen an die Controller-Schicht ergibt sich daher folgende Struktur:

![[Controller-Layer.png]]

Da sich alle Methoden aus den vorangegangenen Methoden der Service-Schicht ableiten, muss hier auf keine Methode im Speziellen eingegangen werden.

### Frontend

Auch die Entwicklung des Frontends basiert auf einem modernen Technologie-Stack, der so im Tagesgeschäft der QuinScape GmbH zum Einsatz kommt. Im Zentrum steht die Verwendung von TypeScript, das als statisch typisierte Erweiterung von JavaScript eine bessere Fehlersuche und eine robustere Codebasis ermöglicht. TypeScript bietet zahlreiche Vorteile, darunter verbesserte Code-Qualität und Wartbarkeit, was insbesondere bei größeren Projekten von großer Bedeutung ist.

Als Framework für die Erstellung der Benutzeroberfläche kommt React zum Einsatz. React ist ein populäres JavaScript-Framework, das die Entwicklung interaktiver und dynamischer Benutzeroberflächen ermöglicht. Mit der Komponentenhierarchie von React können wiederverwendbare UI-Komponenten erstellt werden, was die Entwicklung effizienter und strukturierter gestaltet.

Zur Gestaltung und zum Layout der App wird TailwindCSS verwendet. TailwindCSS ist ein utility-first CSS-Framework, das eine hohe Flexibilität und Kontrolle über das Styling der Komponenten bietet. Es erlaubt den EntwicklerInnen, direkt auf Klassenebene zu arbeiten, was zu einer schnelleren und konsistenteren Gestaltung führt.

Zusätzlich wird das shadcn/ui-Bibliothek integriert, um eine Vielzahl von benutzerdefinierten UI-Komponenten bereitzustellen. Diese Bibliothek ergänzt TailwindCSS und bietet vorgefertigte, stilisierte Komponenten, die einfach integriert und angepasst werden können. Dies beschleunigt die Entwicklung und stellt sicher, dass das Design der App modern und ansprechend ist.

Die Verwaltung der Abhängigkeiten und der Build-Prozesse des Frontends wird mit npm (Node Package Manager) durchgeführt. npm ist ein weit verbreitetes Tool in der JavaScript-Community, das die Verwaltung von Bibliotheken und Tools vereinfacht und eine konsistente Entwicklungsumgebung sicherstellt.

#### Struktur

Bei der Strukturierung des Frontend-Codes wurde nach kurzer Überlegung die Entscheidung getroffen, diesen nach Features zu organisieren. In einer solchen Struktur werden alle Dateien, die zu einem bestimmten Funktionsbereich gehören, gemeinsam in einem Ordner abgelegt. Dies umfasst Komponenten, Styles, Tests und sonstige Ressourcen, die für das jeweilige Feature relevant sind. Durch diese Organisation wird sichergestellt, dass Entwickler alle notwendigen Dateien an einem Ort finden und Änderungen effizient vornehmen können. Darüber hinaus fördert diese Struktur die Modularität des Codes, erleichtert das Auffinden von Abhängigkeiten und trägt dazu bei, dass sich neue Teammitglieder schneller zurechtfinden. Insgesamt bietet diese Herangehensweise eine robuste Grundlage für die skalierbare Entwicklung und Pflege des Frontends.

Diese Struktur lässt sich somit einfach aus der Soll-Analyse deduzieren, da wir dort bereits die zwei Hauptfunktionalitäten der Applikation definiert haben.

#### User Interface
##### Nahrungsmitteldatenbank

Der Entwurf zur Darstellung der Nahrungsmitteldatenbank ist auch hier schnell vollzogen, da das Datenbankmodell alle wichtigen Modularitäten bereits festlegt. Es muss nicht weit von einer tabellarischen Darstellung der einzelnen Nahrungsmittel abgewichen werden, da diese Darstellung auch für die NutzerInnen am intuitivsten ist. Lediglich die Aktionen, mit denen die einzelnen Nahrungsmittel editiert, gelöscht oder zu Logs hinzugefügt werden können, müssen zur Tabelle hinzugefügt werden. Daher ergibt sich der folgende Entwurf:

![[SCR-20240523-kzon-2.png]]

Hier sieht man im oberen Bereich die Funktionalität der Nahrungsmitteldatenbank mit vier Beispieleinträgen. In jeder Zeile kann man den Namen, die Kalorienanzahl und die drei Makronährstoffe des jeweiligen Nahrungsmittels ablesen. Auf der rechten Seite der Tabelle hat jede Zeile jeweils drei Knöpfe: einen Plusknopf, mit dem das Nahrungsmittel zu einem Log hinzugefügt werden kann, einen Editieren-Knopf, mit dem der Datenbankeintrag bearbeitet werden kann, und einen Löschen-Knopf, der das Nahrungsmittel aus der Datenbank entfernt.
##### Logs

Aus dem Entwurf der Nahrungsmitteldatenbank lässt sich auch ein Design für die Logs extrapolieren. Der Plusknopf in den Zeilen kann entfallen, und stattdessen muss die Möglichkeit hinzugefügt werden, ein Log eines bestimmten Datums auszuwählen. Hieraus ergibt sich folgender Entwurf:

![[Log.png]]


Hier sieht man an der obersten Stelle den Knopf, mit dem man einen Datumspicker öffnen kann, um zwischen den einzelnen Logs zu navigieren. Darunter befindet sich eine Auflistung der einzelnen Nahrungsmittel, die bereits in diesem Log gespeichert sind, inklusive eines Zeitstempels zur besseren Organisation, dem Namen des Nahrungsmittels und der Menge. Rechts davon befinden sich nur zwei Knöpfe: ein Knopf zum Bearbeiten des jeweiligen Nahrungsmittels und ein weiterer zum Löschen.

Die Navigationsleiste am unteren Rand der Seite ist in beiden Komponenten gleich. Daraus lässt sich schließen, dass diese übergeordnet angelegt werden kann und nicht Teil der beiden einzelnen Komponenten ist.

##### Formulare

Zwei Komponenten, die den jeweiligen Hauptfunktionen der Applikation untergeordnet sind, fehlen hier noch. Zum einen benötigen wir ein Formular, mit dem sich ein neues Nahrungsmittel in der Datenbank anlegen lässt und mit dessen Hilfe wir bestehende Nahrungsmittel bearbeiten können. Dieses Formular wird dem Feature der Nahrungsmitteldatenbank unterstellt. Andererseits benötigen wir ein weiteres Formular, mit dem sich Nahrungsmittel in ein Log hinzufügen oder dort bereits hinterlegte Nahrungsmittel bearbeiten lassen. Dieses wird folglich dem Feature der Logs untergeordnet.

Die zwei Formulare lassen sich folgendermaßen konzeptualisieren:

![[Create&Add.png]]


#### Komponenten

Einer der Vorteile bei der Entwicklung des Frontends ist, dass man bereits den Großteil des Konzeptes vervollständigt hat, sobald man das User Interface konzeptualisiert hat. Lediglich Helfermethoden fehlen noch, um das Frontend mit der API zu verbinden. Hierfür nehmen wir die im Backend erarbeiteten Endpunkte und implementieren die entsprechenden Axios-Funktionen.

Axios ist eine in der JavaScript-Welt weit verbreitete Bibliothek, die dazu dient, HTTP-Anfragen zu erstellen. Sie bietet eine einfach zu bedienende API, um HTTP-Requests und -Responses zu verwalten. Im Vergleich zu nativen Fetch-Funktionen oder älteren XMLHttpRequest-Objekten ist Axios vielseitiger und bietet viele nützliche Features direkt out-of-the-box. Dazu gehören automatisches JSON-Daten-Parsing, einfaches Handling von Anfragen und Antworten mit Promises sowie die Möglichkeit, Abfangmaßnahmen und Abbruch-Optionen zu definieren. Durch die Verwendung von Axios machen wir den Prozess der Kommunikation mit unserem Backend nicht nur intuitiver, sondern auch robuster und leichter wartbar.

Für unsere Applikation bedeutet das, dass jedes Feature jeweils nur drei Axios-Funktionen benötigt: eine zum "Upserten", eine zum Abrufen und eine zum Löschen. Mit diesen insgesamt nur sechs Aktionen, die auf die API zugreifen, können wir bereits eine funktionierende Applikation mit allen herausgearbeiteten Anforderungen erstellen.

## Implementierungsphase

Während der Implementierung stellte sich heraus, dass einige Ergänzungen und Änderungen an dem Entwurf vorgenommen werden mussten. Diese werden in den folgenden Kapiteln näher erläutert.

### Backend

##### Model

Die Implementierung der Modellschicht verlief ohne Komplikationen, da hier mit der Lombok Java Bibliothek gearbeitet wurde und somit viel Boilerplate-Code vermieden wurde. Notwendige Teile einer Java-Klasse wie Getter- und Setter-Methoden sowie Konstruktoren müssen so nicht mehr selbst geschrieben werden, sondern werden beim Start des Backends generiert.

Lediglich in der Verbindung zwischen den Datenbanktabellen kam es zwischenzeitlich zu Problemen bei der Generierung der JSON-Darstellung von Objekten und beim Abruf von Logs mit mehr als einem Eintrag. Im ersten Entwurf war nämlich geplant, den Java-Code so zu verfassen, dass die FoodItemEntry-Klasse Zugriff auf die NutritionLog-Klasse und die FoodItem-Klasse bekommt und nur durch Annotationen die IDs hinterlegt sind. Dies führte zu unendlicher Rekursion, da jeder Entry Zugriff auf den NutritionLog bekam und beim Abruf dieses Logs wiederum Zugriff auf die darin liegenden Entries nahm.

Hier hätte man mit sogenannten DTOs (Data Transfer Objects) arbeiten können, aber da die Zeit bereits knapp wurde, konnte das Problem auch umgangen werden, indem der Verweis auf die NutritionLog-Klasse entfernt und stattdessen ein Fremdschlüsselfeld verwendet wurde.

Dies ließ sich allerdings nur so leicht umgehen, weil das Datenmodell relativ simpel gehalten ist. Wenn die Applikation in Zukunft wächst und das Datenbankmodell um Ergänzungen bereichert wird, wird man an DTOs nicht vorbeikommen, da diese bei komplexen Backends unumgänglich sind.

##### Repository

Beim Repository lief alles wie im Entwurf geplant und nichts musste abgeändert werden.

##### Service

Die größte Änderung am Backendentwurf findet sich im Erstellen eines neuen Logs. Wie bereits erwähnt, soll es dem Frontend egal sein, ob ein Log bereits existiert, wenn ein Eintrag hinzugefügt wird. Da dies nicht so einfach war wie zuvor angenommen, wurde viel Zeit in die Implementierung dieser Funktionalität investiert, da hier auf viele verschiedene Dinge geachtet werden musste. Die Upsert-Service-Methode musste daher sehr oft umgeschrieben werden und entsprach nach Ablauf der verplanten Zeit noch nicht den sonst sehr akribisch verfolgten Clean Code Prinzipien. Hier muss nach Abgabe des Projekts noch nachgebessert werden, soll die Applikation weiter wachsen und wartbar bleiben.

##### Controller

Auch beim Controller konnte der Entwurf fast deckungsgleich verfolgt werden. Lediglich fiel bei der Implementierung des Frontends auf, dass die Funktionalität zum Löschen und Verändern von Einträgen aus Logs vergessen wurde. Dies hatte zur Folge, dass ein weiterer Endpunkt angelegt werden musste, um Einträge zu löschen.

##### Konfiguration

Ein weiterer Punkt, der bei der Implementierung und Testung des Backends vergessen wurde und erst auffiel, als die ersten Endpunkte mit dem Frontend angesteuert wurden, war, dass eine CORS-Konfiguration fehlte. Damit das Frontend aus dem Browser heraus Zugriff auf die API über den konfigurierten Port hat, muss dieser Port erst freigegeben werden. Dies war glücklicherweise einfach dank Spring Boot. Hier musste lediglich eine Konfigurationsklasse angelegt, mit der Annotation @Configuration versehen und die Methode addCorsMappings der Klasse WebMvcConfigurer überschrieben werden. Hier konnten alle vier benötigten HTTP-Methoden auf den Port des Frontends freigegeben werden.

##### Datenbankinitialisierung

Einer der Vorteile an SQLite3 ist es, dass die Datenbank als Datei direkt ins Backend implementiert werden kann. Damit wir diesen Vorteil auch ausnutzen können, bietet es sich an, die Erstellung und Validierung des Datenbankmodells direkt mit dem Backend selbst durchzuführen. Hierfür wurde eine Klasse namens "DatabaseInitializer" angelegt, die bei jedem Start des Backends aufgerufen wird und prüft, ob alle Tabellen der Datenbank vorhanden sind und diese im Zweifelsfall anlegen kann. Dafür wurden drei Methoden erstellt, die jeweils eine der Tabellen prüfen und anlegen können, wenn diese noch nicht existieren. Dies ist interessanterweise der einzige Ort im gesamten Backend, wo SQL-Code manuell verfasst wurde. Hier ist ein Beispiel für eine solche Methode:

![[DBInitMethodExample.png]]

##### Logging

Um die Fehlersuche beim Programmieren und Ausführen des Codes zu vereinfachen, wurde ein Logger verwendet, der praktischerweise Teil der Lombok-Bibliothek ist. Dieser kann in jede Klasse implementiert werden, indem man dieser die Annotation @Slf4j voranstellt. Damit kann man mit dem Objekt "log" diverse Schweregrade von Meldungen nutzen, wie z.B. log.info oder log.error (siehe vorherige Abbildung). Tritt ein Fehler in einer der vielen Methoden des Backends auf, sieht man so sofort, wo dieser auftrat.

### Frontend

Die Implementierung des Frontends lief zum größten Teil wie im Entwurf geplant ab. Lediglich den beiden Formularen zur Erstellung und Bearbeitung von Nahrungsmitteln und Logeinträgen wurde ein Abbrechen-Knopf hinzugefügt, damit NutzerInnen den Vorgang wieder abbrechen können. Weitere Punkte, die die User Experience verbessern, fielen zwar auf, konnten aber mangels Zeit nicht implementiert werden. Beispielsweise kann man im Datumspicker des Formulars zum Hinzufügen von Logeinträgen noch keinen Zeitstempel auswählen. Dies macht das Feld für den Zeitpunkt obsolet und muss nachgeliefert werden. Außerdem müssen den Löschknöpfen noch Abfragen zur Bestätigung des Löschvorgangs hinzugefügt werden, um versehentliches Löschen von Datenbankeinträgen zu verhindern.

Ein weiterer Punkt ist die fehlende Option zur Auswahl eines Themes. Aktuell ist die Applikation zu 100 % im Dunkelmodus, was zwar dem Geschmack des Entwicklers entspricht, aber nicht alle NutzerInnen bevorzugen diese Farbgebung.

Zudem ist die Applikation zwar für Smartphone-Bildschirme ausgelegt, es werden aber nicht unbedingt moderne Wege zur Datenerfassung auf Smartphones genutzt. Besonders die Formulare müssen dahingehend noch verbessert werden, sodass man z.B. Zahlen nicht mehr mit der Tastatur, sondern mit Swipe-Gesten eingeben kann. Auch die Nutzung von Knöpfen in den Tabellen ist nicht zeitgemäß. Hier wäre es intuitiver, wenn NutzerInnen die Tabellenzeilen anklicken könnten und ihnen dann erst die Zeilenoptionen angezeigt würden.

Eine kleine Abweichung vom Entwurf, um die User Experience zu verbessern, findet sich im Design der Navigationsleiste. Einerseits wurde der Knopf, mit dem man Nahrungsmittel zur Datenbank hinzufügen kann, vergrößert und rund gemacht, wodurch die Optik der Leiste etwas aufgelockert wird. Außerdem wird der Knopf des Features, an dem man sich aktuell befindet, blau eingefärbt. Das hilft, sich intuitiv schneller zurechtzufinden.

#### React-Router

Zur Vereinfachung der Navigation zwischen den Komponenten wurde auf React Router gesetzt. Dies ist eine Bibliothek, die React erweitert. So können in der Hauptkomponente sogenannte Routes konfiguriert werden, die dann von überall aus in der Applikation angesteuert werden können. Ein weiterer Vorteil ist, dass sogar Parameter und Objekte als React Props weitergeleitet werden können. Im Falle dieser Applikation bedeutet das z.B., dass wir eine Route "nutrition-log/:date?" konfigurieren können, die dann die Möglichkeit bietet, direkt das Datum des gewünschten Logs in der Navigationsleiste aufzurufen. Ruft die App zum Beispiel die URL "nutrition-log/2024-05-27" auf, landet man automatisch im Log des 27.05.2024. Das vereinfacht die Weitergabe von Daten innerhalb der App enorm, da React Props und State nicht mehr manuell durch die einzelnen Komponenten getragen werden müssen.

Ein weiterer Vorteil von React Router ist, dass wir das Location-Interface direkt als Parameter in React Hooks wie useEffect() nutzen können. Dadurch kann z.B. eine useEffect-Funktion geschrieben werden, die die übergeordnete Komponente immer dann neu rendert, sobald mit React Router eine neue URL aufgerufen wird (auch wenn es sich um dieselbe URL handelt, die gerade aufgerufen ist). Ein Nachteil von React ist nämlich, dass das Neuladen von Komponenten nicht immer so einfach ist, wie man denkt. Löscht man beispielsweise einen Eintrag aus der Datenbank, möchte man aus UX-Perspektive, dass dies auch sofort als Feedback zurückgegeben wird. Dies kann mit React Router sehr einfach realisiert werden, indem man bei jedem Löschvorgang die Komponente neu lädt.

#### Nahrungsmitteldatenbank

![[Foods.png]]

Die Texte auf den Knöpfen wurden hier zu Icons abgeändert, um das Design so prägnant und einfach verständlich wie möglich zu halten. Sonst wurde das Design des Entwurfes fast vollständig übernommen.

#### Logs

![[Log App.png]]

Hier findet man einige Abweichungen zum ursprünglichen Frontend-Entwurf. Neben den Icons, die mit Logos getauscht wurden, gibt es einen zusätzlichen Bereich, in dem die Summen der Kalorien und Makronährstoffe abgelesen werden können. So hat man in jedem Log sofort die gewünschten Daten zur Hand. Dieser Bereich ist natürlich das Herzstück der App und darf nicht fehlen, sonst ergibt das Nachhalten der Nahrungsmittel keinerlei Sinn. NutzerInnen, die Gewicht verlieren möchten, sind auf die Summe der Kalorien angewiesen.

Dieser Punkt wurde im Entwurf des Backends eigentlich bedacht, da die Hilfsmethode zur Berechnung der Summen von Anfang an eingeplant war. Ein entsprechender Bereich wurde beim Frontend-Entwurf dann lediglich vergessen. Auch hier gibt es in Zukunft in Sachen UX noch Nachholbedarf. Zahlen als solche sind weniger intuitiv und sollten mit Fortschrittsbalken versehen werden, an denen man sofort erkennen kann, wie nah man sich an den täglichen Grenzen oder Zielen befindet.

#### Formulare

![[Add Food.png]]

Auf diesem Bild kann man leider nicht das ganze Formular erkennen, da dieses länger als der Bildschirm ist, aber unter dem Kohlenhydrat Feld befinden sich noch die zwei genannten Submit- und Cancel-Knöpfe. Diese kann man auf dem nächsten Bild sehen:

![[Add Entry.png]]

Bei diesem Formular gibt es eine kleine Abweichung vom Entwurf. Statt "Entry" steht in der Überschrift der Name des Nahrungsmittels, das man zum Log hinzufügen möchte. Dies hilft den NutzerInnen zu sehen, dass sie auch das richtige Nahrungsmittel ausgewählt haben. Realisiert wurde dies mithilfe von React, indem man den State des aktuellen Nahrungsmittels ausliest und direkt als HTML zurückgibt.

Gerade die Implementierung der Formulare hat im Bereich des Frontends die meiste Zeit in Anspruch genommen. Hier wurde nach der Dokumentation der Komponentenbibliothek shadcn/ui gearbeitet, wodurch noch weitere Bibliotheken herangezogen werden mussten. Formulare sind im Internet zwar eine der gebräuchlichsten Funktionalitäten, aber gerade in Kombination mit React stellen sie eine der größten Hürden dar. Dies hat einerseits den Hintergrund, dass die gebräuchlichsten Attacken auf die Sicherheit einer Seite über Formulare erfolgen, und andererseits werden Formulare in React "kontrolliert" realisiert. Das bedeutet, dass jede Änderung des Inhalts eines Formularfelds ein Event aufruft, im Gegensatz zum gebräuchlichen Weg, bei dem ein Event erst aufgerufen wird, wenn die NutzerInnen auf den Senden-Knopf drücken.

Die Formularbibliothek ZOD versucht dies einerseits zu vereinfachen und bietet zudem die Funktionalität, Formularfelder direkt bei der Eingabe auf korrekte Daten zu überprüfen. Hier wurde es so realisiert, dass Zahlenfelder wirklich nur Zahlen akzeptieren, diese Zahlen positiv sein müssen, das Kalorienfeld mindestens 1 betragen muss und das Unit-Feld lediglich zwei verschiedene Zustände hat (Gramm oder Milliliter). Das hat aber auch zur Folge, dass man zusätzliche Datentypen, Interfaces und Schemata erzeugen muss, damit diese Typensicherheit im Hintergrund ohne Probleme gewährleistet ist.

## Testphase

Wie der Projektplanung entnehmbar ist, lief der Großteil der Testphase bereits während der Implementierungsphase ab. Besonders im Falle des Backends wäre es kaum sinnvoll gewesen, erst alle Endpunkte anzulegen und diese dann erst gebündelt zu testen. Auch wenn das Backend nach Schichten strukturiert ist, wurde es dennoch nach Features implementiert, sodass nach jedem abgeschlossenen Feature dieses direkt getestet werden konnte. Für das Backend wurde hierfür das Tool Postman herangezogen.

**Postman** ist ein weit verbreitetes und leistungsfähiges Tool, das EntwicklerInnen dabei hilft, APIs zu testen. Es ermöglicht das Senden von HTTP-Anfragen und das Visualisieren der Antworten in einer benutzerfreundlichen Oberfläche. Mit Postman können Entwickler schnell und effizient verschiedene Szenarien durchspielen, indem sie GET-, POST-, PUT- und DELETE-Anfragen testen. Es bietet zudem die Möglichkeit, Anfragen zu speichern und als Sammlungen zu organisieren, was besonders nützlich für die Wiederverwendung und Dokumentation ist. Darüber hinaus unterstützt Postman das Testen von Endpunkten mit verschiedenen Parametern und Headern sowie die automatische Generierung und Auswertung von Testscripten, um die Vollständigkeit und Richtigkeit der API sicherzustellen. Der Einsatz von Postman in der Testphase sorgte somit für eine systematische und gründliche Überprüfung der Funktionalität des Backends und trug maßgeblich zur Qualitätssicherung bei.

So wurde nach jeder Implementierung eines API-Endpunktes dieser mit Test-Requests in Postman angesteuert. Dadurch konnte sofort erkannt werden, wenn ein Endpunkt nicht wie gewünscht funktionierte.

Sobald ein Fehler gefunden wurde, wurde außerdem in die Logs des Backends geschaut und mit dem Debugger von IntelliJ IDEA nach den Gründen dafür geforscht. Besonders beim Implementieren der upsert-Methoden wurde dieser intensiv zu Rate gezogen, um sicherzustellen, dass die Implementierung korrekt und stabil ist.

## Übergabe

Nach Abschluss des letzten Sprints wurde die Anwendung zur endgültigen Abnahme Herrn Hillman vorgelegt. Die Endabnahme lief, durch die SCRUM typischen vorherigen Iterationen der Sprint Reviews, problemlos.


# Fazit

## SOLL/IST Vergleich

Alle im SOLL-Kapitel geplanten Ziele wurden erreicht. Hierbei kam es zu keinen Abweichungen in der Zeitplanung. Zunächst schien es bei der Implementierung so, als würde noch viel Zeit übrig bleiben, um weitere UI/UX-Verbesserungen vornehmen zu können, die auf jeden Fall noch in Zukunft nötig sein werden. Durch die Implementierung mancher komplizierter Funktionalitäten im Frontend und Backend wurde jedoch mehr Zeit für das Debuggen benötigt als ursprünglich angenommen. Besonders die Implementierung der upsert-Servicemethoden im Backend und das Realisieren der Komponentenbibliothek in Verbindung mit Formularen und Tabellen im Frontend haben die zunächst eingesparte Zeit vollständig aufgebraucht.

## Erkenntnisse

Bei der Durchführung des Projekts fiel vor allem auf, wie schwierig es ist, ein Projekt eigenständig zu planen und sich an diese Planung zu halten. Hierbei waren vor allem die täglichen Sprint-Meetings eine große Hilfe, um die Arbeit des vergangenen Tages Revue passieren zu lassen und die Arbeit der folgenden 8 Stunden organisiert zu strukturieren. Eine vollständige Applikation zu entwickeln, inklusive Backend und Frontend, war eine wichtige Erfahrung auf dem Weg, ein vollwertiges Mitglied in zukünftigen Entwicklerteams zu werden.

Besonders das Arbeiten mit Spring Boot, JPA und Lombok im Backend sowie das Anbinden des React-Frontends mit Axios und das Verfassen von Frontend-Code mit TypeScript waren wichtige Erfahrungen, die den eigenen Horizont erheblich erweitert haben.

## Ausblick

Wie aus der Dokumentation zu entnehmen sein sollte, fehlen noch einige Funktionalitäten in der Applikation. Zu den angesprochenen UI/UX-Verbesserungen im Frontend, wie z.B. moderne UI-Komponenten, die besser an Smartphones und Touchscreens angepasst sind, sowie ein fehlender Hellmodus, kommt vor allem die fehlende Funktionalität, Nutzervorgaben einzugeben.

Beim Abnehmen ist es z.B. wichtig, das eigene Gewicht nachzuhalten, Kaloriengrenzen zu setzen und Makronährstoffvorgaben zu berechnen. Daraus lässt sich der Nutzen einer Nutzerdatenbank ableiten, was wiederum die Erweiterung der Applikation um Authentifizierungs- und Autorisierungsfunktionalitäten erforderlich macht. Dies könnte im Backend mit Spring Security realisiert werden, das während der Entwurfsphase zwar in Erwägung gezogen wurde, aber aufgrund der knappen Zeitplanung gestrichen werden musste.

Sollte man diese App in Zukunft der breiten Öffentlichkeit zur Verfügung stellen wollen, würden die NutzerInnen nicht alle gebräuchlichen Nahrungsmittel händisch hinzufügen wollen. Hier wäre es sinnvoll, die Nahrungsmitteldatenbank an öffentliche Datenbanken anzuschließen, die bereits die meisten Nahrungsmittel enthalten (z.B. Openfoodfacts oder die US-amerikanische Nahrungsmitteldatenbank).

Es gibt also noch viele Erweiterungen, an denen in Zukunft sicherlich weiter gearbeitet werden kann. Diese Verbesserungen und zusätzlichen Funktionalitäten würden die Applikation umfassender und benutzerfreundlicher machen und sie so zu einem wertvolleren Tool für die NutzerInnen entwickeln.

# Literaturverzeichnis

