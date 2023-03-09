das Anwesenheitsboard hier im Bereich Lindemannstrasse hat sich offensichtlich mal wieder aufgehangen, jedenfalls ist nur noch der Screen "Gehört dieses Tag XY" zu sehen und es reagiert nicht mehr auf Eingaben.

Da das jetzt schon mehrfach vorgekommen ist mit unterschiedlichen Fehlerbildern:
-   Falls noch nicht geschehen: Logging der Anwendung erweitern oder anschauen um diese Fehler endlich auszumerzen. Kann nicht sein, dass eine so einfache Applikation so oft hängenbleibt und wir das nicht gefixt bekommen. (**Team Anwesenheitsboard**).
-   Eine bessere Dienstüberwachung implementieren, damit sowas besser "erkannt" wird und nicht erst ein Ticket geschrieben werden muss:
-   a) Dienst läuft (bzw. nicht), Hardware-Umgebung läuft/läuft nicht
-   b) "Dienst läuft aber es ist seit zu langer Zeit nichts passiert im Board (weil keine Anmeldungen oder Abmeldungen stattfanden, obwohl es ein Nicht-Feiertag ist und das eigentlich nicht sein kann".
-   (**Team Anwesenheitsboard zusammen mit IT**)

https://intern.quinscape.de/confluence/pages/viewpage.action?pageId=115867977

https://intern.quinscape.de/bitbucket/projects/CA/repos/attendanceboard/browse

## Beobachtungen

- less statt css
- typescript
- Gradle Build -> Backend (Spring)
	- install: `./gradlew build`
	- start: `./gradlew startFrontend`
- npm -> Frontend (Angular)
	- install: `./src/main/webapp npm install`
	- start: `./gradlew startBackend`

- Funktioniert nicht mit Java 17. Keine Probleme mit Java 11.
	- Error: `java.lang.NoClassDefFoundError: Could not initialize class org.codehaus.groovy.vmplugin.v7.Java7`

Besprechung 08.03.2023
- Email Verteiler für Anwesenheitsboard erstellen
- Eigenes Team in Teams erstellen
- Tickets in Jira -> Rückmeldung geben, wenn es geklärt ist
- Anwesenheitsboard mit AD verknüpfen? User Datenbank zum Abgleich
	- Frontend überarbeiten, dass neue Mitarbeiter sich direkt anmelden können (Tag mit User verbinden)
- Prio1: Monitoring ermöglichen: Endpunkte zum Auslesen des Gesundheitsstatus' implementieren
- Prio2: Skripte zum Neustarten/Fehler beheben
- Zweites Board läuft unbenutzt in der IT, wenn es zum Fehler kommt, kann man das besser analysieren