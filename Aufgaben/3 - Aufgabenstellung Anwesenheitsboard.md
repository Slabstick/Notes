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
	- nicht kompatibel mit neuen npm versionen. Muss mit NVM auf Version 14.21.3 laufen:
	- `nvm use 14.21.3`
	- install: `./src/main/webapp npm install`
	- start: `./gradlew startBackend`

- Funktioniert nicht mit Java 17. Keine Probleme mit Java 11.
	- Error: `java.lang.NoClassDefFoundError: Could not initialize class org.codehaus.groovy.vmplugin.v7.Java7`



### Besprechung 08.03.2023
- Email Verteiler für Anwesenheitsboard erstellen
- Eigenes Team in Teams erstellen
- Tickets in Jira -> Rückmeldung geben, wenn es geklärt ist
- Anwesenheitsboard mit AD verknüpfen? User Datenbank zum Abgleich
	- Frontend überarbeiten, dass neue Mitarbeiter sich direkt anmelden können (Tag mit User verbinden)
- Prio1: Monitoring ermöglichen: Endpunkte zum Auslesen des Gesundheitsstatus' implementieren
- Prio2: Skripte zum Neustarten/Fehler beheben
- Zweites Board läuft unbenutzt in der IT, wenn es zum Fehler kommt, kann man das besser analysieren

### Onboarding 10.03.23
Link zum Attendanceboard (intranet): https://intern.quinscape.de/attendanceBoard/main#A
Login: attendanceboard
PW: attendanceboard20

Verbindung per: `ssh jklimczok@awboard-server-vm.qs.intra`


05.04.23

Passwort Dokumentation überarbeiten
AB Update durch IT im JIRA dokumentieren

04.05.23

Autologin: MUSS auf  /main redirecten. index.html redirected zur Loginseite.
Wenn Login im Localstorage gespeichert wird, wird kein Cookie mit der SessionID gesetzt??

26.06.23
Autoneustart der Clients/(Server?) jeden Sonntag implementieren

5.7.23
Verortung der MA nicht nach Anmeldedaten, sondern an welchem Client man sich anmeldet.

6.07.23 - Bilder hochladen

Bilder lassen sich nicht mehr hochladen!

![[MicrosoftTeams-image (2).png]]

Mit CSS auf Hintergrund legen:

``` HTML
<!DOCTYPE html>  
<html>  
<head>  
<style>  
#grad1 {  
  height: 200px;  
  background-color: green; /* For browsers that do not support gradients */  
  background-image: linear-gradient(to right,#0220B1, transparent);  
}  
</style>  
</head>  
<body>

<h1>Linear Gradient - Top to Bottom</h1>  
<p>This linear gradient starts red at the top, transitioning to yellow at the bottom:</p>

<div id="grad1"></div>

</body>  
</html>
```


16.08.2023
- Wir haben Zugriff auf die Steckdose, also Neustarten sollte über VNC gehen.
- Maynard final testen und IT Bescheid geben
- SNOOPY zeitnah (nach kurzer Testphase auf MAYNARD) auf Linux umrüsten


## 22.08.2023
### Autorestart
- Autorestart jeden Sonntag um 3 Uhr Nachts (3am):
- 2 Scripts in /etc/systemd/system/:

autorestart.service:
```ini
[Unit]
Description=Reboot the system every Sunday at 3 AM

[Service]
Type=oneshot
ExecStart=/sbin/shutdown -r now "Rebooting the system at 3 AM"

```

autorestart.timer
```ini
[Unit]
Description=Reboot the system every Sunday at 3 AM

[Timer]
OnCalendar=Sun *-*-* 03:00:00
Persistent=true

[Install]
WantedBy=timers.target

```

- gestartet und enabled:

```bash
sudo systemctl enable autorestart.timer
sudo systemctl start autorestart.timer
```

- Kann gecheckt werden per:

```bash
sudo systemctl status autorestart.timer
```

### VNC Server Troubleshoot/Wartung

- in /home/snoopy liegt eine Datei namens .Xauthority, welche owner snoopy und gruppe snoopy haben MUSS und rw Nutzerrechte haben MUSS

```bash
ps aux | grep Xorg
```

- Zeigt alle bestehenden und offenen Xorg Sitzungen an. 
- tty2 Sitzung auf snoopy: muss vorhanden sein. Wenn nicht muss GMD restartet werden

```bash
sudo systemctl restart gdm.service
```

- in `azubi/.vnc/`  liegen logs der einzelnen Monitore (`snoopy:n.log` wobei n für den Monitor steht)
- in `azubi/xlvnc.log` sind die Server Logs

### First Responder Botmessage

