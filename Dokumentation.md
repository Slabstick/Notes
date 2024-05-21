
# Inhaltsverzeichnis
Abbildungsverzeichnis
Tabellenverzeichnis
Listings
Abkürzungsverzeichnis

# Einleitung
## Projektumfeld

Die QuinScape GmbH ist ein deutscher IT-Dienstleister, welcher bereits seit über 20 Jahren als Spezialist in den Themenbereichen Data & Analytics und Software Engineering aktiv ist. Mit Hilfe der Vielzahl an Partnern und den mittlerweile über 200 MitarbeiterInnen, die in dem Hauptsitz Dortmund, sowie dem Nebenstandort Hannover tätig sind, realisiert das Unternehmen individuelle Lösungen für die anspruchsvollen Bedürfnisse seiner KundInnen. Seit 2021 agiert die QuinScape GmbH außerdem als Gründungsunternehmen der Dataciders GmbH (ehemals QuinScape Group), die mittlerweile sechs weitere Unternehmen der IT-Branche beinhaltet. Die Dataciders GmbH beschäftigt insgesamt über 500 Personen aus mehr als 15 Nationen.


## Ausgangssituation

Viele Menschen haben Schwierigkeiten, ihre Ernährungsgewohnheiten zu überwachen und gesundheitliche Ziele zu erreichen, da sie oft nicht über die notwendigen Informationen oder Werkzeuge verfügen, um ihre Nahrungsaufnahme effektiv zu verfolgen. Besonders die Wahl von kalorienarmen Nahrungsmitteln fällt vielen Menschen schwer, da sie im Supermarkt durch Werbung, Marketing und offizielle Qualitätssiegel und Verpackungsaufdrucke verwirrt und oft auch getäuscht werden.

## Projektbeschreibung

Bei dem vorgestellten Projekt handelt es sich um ein eigenständiges Projekt, welches intern in der Software Engineering Abteilung der QuinScape GmbH entwickelt wird. Die Anforderungen an das Projekt werden von meinem Ausbilder Florian Hillmann gestellt, welcher als Kunde auftritt.

In diesem Projekt soll eine webbasierte Anwendung entwickelt werden, die Nutzern ermöglicht, ihre tägliche Nahrungsaufnahme zu verfolgen und detaillierte Informationen über die Nährwerte ihrer Mahlzeiten zu erhalten. Ziel ist es, das Bewusstsein und das Verständnis der Nutzer für ihre Ernährung zu verbessern und sie bei der Erreichung ihrer gesundheitlichen und fitnessbezogenen Ziele zu unterstützen.

## Projektziel

Das Hauptziel dieses Projektes ist die Entwicklung einer intuitiven und benutzerfreundlichen Anwendung, die es Nutzern nicht nur ermöglicht, ihre tägliche Kalorienaufnahme einfach zu protokollieren und zu überwachen, sondern auch einen Einblick in ihre Makronährstoffverteilung (Proteine, Kohlenhydrate, Fette) gibt. Diese Funktionalität ist essentiell, um nicht nur Gewichtsverlustziele zu unterstützen, sondern auch spezifische Fitness- und Gesundheitsziele, wie den Muskelaufbau oder die Verbesserung der allgemeinen Körperzusammensetzung, zu erreichen.

Die Anwendung bietet eine Datenbank mit Nahrungsmitteln, die detaillierte Informationen zu Kalorien und Makronährstoffen enthält. Nutzer können durch diese Datenbank nach bereits gespeicherten Nahrungsmitteln suchen, um ihre täglichen Mahlzeiten zusammenzustellen, oder eigene Nahrungsmittel hinzufügen, falls diese nicht vorhanden sind. Jedes Nahrungsmittel kann mit der entsprechenden Menge zum persönlichen Ernährungstagebuch hinzugefügt werden, welches automatisch die Summe der konsumierten Kalorien und Makronährstoffe für den Tag berechnet.

Die Benutzeroberfläche ist darauf ausgelegt, den Ablauf so einfach wie möglich zu gestalten. Nutzer können direkt von der Startseite aus auf die Funktionen zum Hinzufügen von Mahlzeiten, Durchsuchen der Nahrungsmitteldatenbank und Anzeigen ihres Ernährungstagebuchs zugreifen. Das Tagebuch präsentiert eine klare und verständliche Zusammenfassung der täglichen Nahrungsaufnahme. Ob es darum geht, Gewicht zu verlieren, Muskelmasse aufzubauen oder einfach eine ausgewogenere Ernährung zu pflegen, die App bietet die Werkzeuge, die Nutzer benötigen, um informierte Entscheidungen über ihre Ernährung zu treffen und ihre Gesundheits- und Fitnessziele zu erreichen.

## Projektschnittstellen

### Personenschnittstellen

### Technische Schnittstellen

## Projektabgrenzung

### Unterschiede zu Projektantrag

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

Für das Styling der Anwendung wurde das Utility-First CSS-Framework Tailwind CSS verwendet. TailwindCSS ermöglicht ein schnelles und effizientes Erstellen von benutzerdefinierten Designs direkt im HTML-Markup, indem es eine Vielzahl von vorgefertigten CSS-Klassen bereitstellt, die einzeln oder in Kombination genutzt werden können. Im Gegensatz zu traditionellen CSS-Frameworks bietet Tailwind CSS keinen vordefinierten Designstil, sondern gibt Entwicklern die Flexibilität, ihr eigenes Designsystem zu erstellen und gleichzeitig konsistente und wartbare Stile sicherzustellen. Durch die Verwendung von Tailwind CSS können spezifische Designs ohne die Notwendigkeit, benutzerdefiniertes CSS zu schreiben, schnell prototypisiert und umgesetzt werden. Dies führt zu einer sauberen, minimalen Stylesheet-Datei und einer besseren Performance der Anwendung. Zudem ermöglicht das aufeinander abgestimmte Ecosystem von Tailwind CSS, einschließlich Plugins und Integrationen, eine nahtlose Anpassung und Erweiterung der Funktionalität.

### Shadcn/ui

Für die Benutzeroberfläche wurde das Shadcn/ui-Framework eingesetzt. Shadcn/ui ist ein modernes UI-Framework, das sich durch seine hohe Anpassungsfähigkeit und Benutzerfreundlichkeit auszeichnet. Es bietet eine Vielzahl von vorgefertigten Komponenten, die leicht in bestehende Projekte integriert werden können, und ermöglicht es Entwicklern, schnell und effizient ansprechende Benutzeroberflächen zu erstellen. Shadcn/ui unterstützt eine komponentenbasierte Architektur und bietet umfangreiche Möglichkeiten zur Anpassung der Komponentenstile, wodurch eine konsistente und individuell gestaltbare UI gewährleistet wird. Durch die Nutzung dieses Frameworks können Entwicklungszeiten reduziert und die Wartbarkeit der Anwendung verbessert werden. Mit Shadcn/ui kann die Produktivität gesteigert werden, während gleichzeitig eine hohe Qualität und Benutzerfreundlichkeit der Benutzeroberfläche sichergestellt wird.

### NPM

Neben den Hauptbibliotheken und Frameworks wurden auch verschiedene kleinere Pakete aus dem Node Package Manager (NPM) Repository integriert, um spezifische Funktionalitäten zu ergänzen und die Entwicklung zu erleichtern. NPM ist das weltweit größte Software-Registry, die es Entwicklern ermöglicht, Open-Source-Pakete einfach zu suchen, zu installieren und zu verwenden. Die Auswahl an Paketen bietet eine breite Palette von Lösungen für Probleme wie etwa Form-Handling, Validierung, Zustandmanagement und Animationen. Durch die Nutzung dieser Pakete konnte die Entwicklungszeit verkürzt und die Codequalität verbessert werden. Die modularen und gut dokumentierten NPM-Pakete tragen zur Flexibilität und Erweiterbarkeit der Anwendung bei, indem sie es ermöglichen, standardisierte und geprüfte Lösungen zu integrieren, ohne von Grund auf neu schreiben zu müssen.

### Git

Für das Versionsmanagement und die Zusammenarbeit im Entwicklungsteam wurde Git als Versionskontrollsystem verwendet. Git ist ein verteiltes Versionskontrollsystem, das eine vollständige Historie aller Änderungen an der Codebasis ermöglicht und somit die Nachverfolgbarkeit und Wiederherstellbarkeit früherer Versionen sicherstellt. Es unterstützt eine effiziente und kollaborative Arbeitsweise, indem es Entwicklern ermöglicht, gleichzeitig an verschiedenen Features und Bugfixes zu arbeiten, ohne sich gegenseitig zu behindern. Das Branching-Modell von Git erleichtert den Workflow erheblich, da Änderungen isoliert vorgenommen und nur dann in den Hauptzweig integriert werden, wenn sie stabil und getestet sind. Darüber hinaus wurde Bitbucket genutzt, um Code-Repositories zentral zu hosten und die später evtl. noch relevante Integration von CI/CD-Pipelines zu unterstützen. Bitbucket erleichtert nicht nur das Code-Review und das Management von Pull Requests, sondern bietet auch Tools zur Automatisierung von Tests


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

## Ablaufplan

## Terminplanung

## Kostenplanung

### Projektkosten

# Durchführung und Auftragsbearbeitung

## Analysephase 

### IST-Analyse

### SOLL-Analyse

### Zieldefinition

## Planungsphase

## Entwurfsphase

### Backend

### Frontend

## Implementierungsphase

## Testphase

## Black-Box-Test

## Schlussphase

## Übergabe

# Fazit

## Erkenntnisse

## Ausblick

# Literaturverzeichnis

