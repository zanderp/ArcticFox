# ArcticFox
*[NFE Team](http://nfeteam.org) präsentiert eine angepasste Firmware für Joyetech, Wismec and Eleaf Akkuträger*

![](http://i.imgur.com/JP4KC8A.png)
![](http://i.imgur.com/E1e7cs1.png)

![](http://i.imgur.com/kYJcp6I.png)
![](http://i.imgur.com/TnqNYK1.png)
![](http://i.imgur.com/0XTV9xD.png)

**[NFE Toolbox](https://github.com/TBXin/NFirmwareEditor/releases) wird für das [Installieren](https://github.com/maelstrom2001/ArcticFox/wiki/How-to-install) der Firmware und die Konfiguration des Gerätes benötigt.**

## Unterstützte Akkuträger:
### Joyetech:
* eVic VTC Mini
* eVic VTC Dual
* eVic VTwo Mini
* eVic VTwo
* eVic AIO
* eVic Basic
* eGrip II / Light
* Cuboid Mini
* Cuboid
* Cuboid 200

### Wismec:
* Presa TC75W
* Presa TC100W
* Reuleaux RX75
* Reuleaux RXmini
* Reuleaux RX200
* Reuleaux RX200S
* Reuleaux RX2/3
* Reuleaux RX300
* VF Lite
* VF Stout
* VF Classic
* BV Centurion
* La Petite Box

### Eleaf:
* Aster
* iStick Pico 75W
* iStick Pico Mega 80W
* iStick Pico Dual
* iStick TC100W
* iStick TC200W
* iStick iPower 80W

## Einschränkungen
Sicherheit bei der Benutzung unserer Firmware ist eines unserer Hauptziele. Alle Begrenzungen des Herstellers werden beibehalten, da sie nicht ohne Grund existieren.

Was sind Einschränkungen?
* Minimaler Widerstand (Für alle unterstützten Akkuträger)
  * 0.05 Ohm für Temperaturmodus
  * 0.1 Ohm für Wattmodus
* Ausgangsleistung (Geräteabhängig)
* Maximaler Ladestrom (Geräteabhängig)
* Maximaler Ausgangsstrom (Geräteabhängig)
* Ausgangsspannungsbereich (Geräteabhängig)

"Geräteabhängig" bedeutet, dass jeder Akkuträger eigene, vom Hersteller festgelegte, Grenzwerte hat. Die genauen Werte lassen sich der Produktbeschreibung des Herstellers entnehmen.

**Alle Anfragen diese Werte anzupassen werden abgelehnt, da es nicht gewünscht ist, dass Benutzer der Firmware sich oder andere zu Schaden bringen.**

## Profile
Eines der Hauptmerkmale der Firmware ist das Profil-basierte Benutzerinterface (DNA-artig), sowie die Ausrichtung auf die Einstellbarkeit im Gegensatz zur originalen Joyetech-Firmware.
Profile sind eine Sammlung von Parametern bezüglich der verwendeten Verdampfer, wie etwa Drahtart, Wicklungswiderstand, Leistungs- und Temperaturwerte.
Der Benutzer hat 8 Profile zur Auswahl, die mit NFE Toolbox bearbeitet und dann den verschiedenen Verdampfern zugewiesen werden können.

![](http://i.imgur.com/UjtY7Ir.png)

Profile können entweder automatisch gewechselt werden, in Abhängigkeit des Widerstands der Wicklung, oder manuell. Um das automatische Wechseln des Profils zu nutzen muss lediglich der "Smart" Modus aktiviert, ein Verdampfer aufgeschraubt und das gewünschte Profil ausgewählt und damit dem Verdampfer zugewiesen werden.

![](http://i.imgur.com/fadryzQ.png)

Beim nächsten Aufschrauben dieses Verdampfers wird das eingestellte Profil automatisch aktiviert.
Wird der Widerstand des Verdampfers nicht in den Profilen gefunden, wird der Benutzer aufgefordert ein neues Profil zu erstellen oder ein existierendes zuzuweisen.
Bei einem manuellen Profilwechsel mit abweichenden, gespeicherten Widerständen, wird der Benutzer aufgefordert ein Profil zu aktualisieren oder die Werte des aktiven Profils beizubehalten.

## Hauptmenü

Gleichzeitiges Betätigen des Feuertasters und der Plus-Taste für eine Sekunde öffnet das Hauptmenü:

![](http://i.imgur.com/XSWOLDJ.png)

## Profilmenü

![](http://i.imgur.com/HOO0KiF.png) ![](http://i.imgur.com/2UPcLHy.png) ![](http://i.imgur.com/yNH5crk.png) ![](http://i.imgur.com/kc0PYf7.png) ![](http://i.imgur.com/CNzn7vQ.png) ![](http://i.imgur.com/3MHoldt.png)

* **Wire** - Drahtmaterial, Temperaturabhängig oder nicht (VW), entweder Standard oder eigene TFR-Werte;
* **Coil** - Gespeicherter Widerstand;
* **TCR** - Werte können bearbeitet werden, wenn der Joyetech TC Algorithmus mit eigener TCR ausgewählt ist;
* **T. Dom** - Temperatur-dominante Regulierung;
* **Preheat** - Leistungskontrolle, entweder Preheat oder Leistungskurve;
* **PI-Reg** - PI Regulator für TC modus, verbessterte, stabilisierte Leistungs- und Temperaturregulierung:
     - PI-Reg On/Off - Wechsel zwischen Joyetech TC Algorithmus und PI Regulierung;
     - Range - 0..100% - Temperaturbereich in dem PI Regulierung aktiv ist. 0 bedeutet, der Regulator ist immer aktiv und kontrolliert die Leistungsabgabe von Beginn des Zuges. 20% bedeutet: PI Regulierung wird aktiv wenn 20% der im Profil eingestellten Temperatur erreicht werden;
     - P - proportionale Konstante, je größer, desto drastischer die Leistungsänderung;
     - I - integrale Konstante, je größer, desto gleichmäßiger ist die Leistungsregelung.

## Screenmenü

![](http://i.imgur.com/6jddZL9.png) ![](http://i.imgur.com/3fRgkGN.png) ![](http://i.imgur.com/FmVjNro.png) ![](http://i.imgur.com/2UYldpC.png)

* **Dim** - Zeit bis zum Abdunkeln des Displays;
* **Wake <>** - Einstellung ob Plus- und Minustaste das Display aufwecken;
* **Charge** - Anzeigen von zusätzlichen Informationen auf dem Ladebildschirm, Batteriespannung(en) und Temperatur des Boards;
* **Logo** - Logo auf dem Hauptbildschirm anzeigen;
* **Clock** - Einstellungen zur Uhr:
     - Type - Analog oder Digital;
     - On Main - Uhr auf dem Hauptbildschirm anzeigen;
     - Saver - Uhr im Standbymodus anzeigen;
* **Contrast** - Helligkeit des Displays justieren;
* **Skin** - Stil des Hauptbildschirms wechseln.

## Einstellungen/Settings

![](http://i.imgur.com/aDuSk3n.png) ![](http://i.imgur.com/3JeWUqf.png) ![](http://i.imgur.com/8V1VCeo.png)

* **1 Watt** - Leistung in 1 Wattschritten ändern;
* **Menu** - New - Profile durch Smartauswahl wechseln, Old - Profile durch normales Editieren/Edit Main wechseln;
* **Smart** - Einstellungen zur automatischen Profilauswahl:
     - On/Off; - Smartauswahl an/aus
     - resistance tolerance; - Toleranzbereich zur Profilauswahl durch Widerstand
     - show Profile Menu after assigning new; -Profilmenü nach Auswahl anzeigen
* **Clicks** - Aktionen die auf 2/3/4 Feuertaster-Klicks liegen:
     - None; - Keine
     - Edit Main - Joyetech reguläre 3-Klick Aktion;
     - Profiles - Profilauswahl;
     - T. Dom - Temperatur-dominante Regulierung an/aus;
     - Clock - Zeige/Verstecke Uhr im Hauptbildschirm;
     - On/Off - Akkuträger ein/ausschalten;
     - LSL - "Light Sleep Mode" aktivieren/deaktivieren; 
     - Main Menu - Hauptmenü öffnen, wie Feuer- und Plustaste betätigen;
     - Preheat - Preheateinstellungen des aktiven Profils;
     - Edit Profile - Profilmenü öffnen;
     - Smart On/Off - Smartmodus ein/aus
     - Show Info Screen - Infobildschirm anzeigen
* **RTC** - RTC (Realtime Clock) Einstellungen;
* **Expert** - Einstellungen für fortgeschrittene Benutzer:

![](http://i.imgur.com/UZBrHjJ.png) ![](http://i.imgur.com/7fT0pNi.png) ![](http://i.imgur.com/edejq3z.png) ![](http://i.imgur.com/FoH1vaE.png)

* **USB**
     - NoSlp - Bei USB-Verbindung nicht in den Schlafmodus wechseln;
     - Charge - Aufladen über USB-Verbindung aktivieren/deaktivieren;
* **BVO** - Batteriespannungskorrektur;
* **BATT** - Entladeprofil für Batterie;
* **SHUNT** - Ohm-meter Korrektur;
* **ChkTCR** - Prüfen der Draht-TCR, Ausschalten kann TCR Error bei großen Coils umgehen;
* **RCOBC** - Puff Counter bei Batteriewechsel zurücksetzen, Zurücksetzen der Vaping Statistiken;
* **X32** - RTC Modul verwendet zusätzlichen 32768 Hz Oszillator, falls vorhanden;
* **LSL** - Light Sleep Mode, für Akkuträger ohne zusätzlichen Oszillator, hält Uhr genau, benötigt etwas mehr Energie im Ruhezustand, daher wird der User durch ein ! rechts der Batterieanzeige gewarnt;
* **TEMP** - Boardtemperatursensor, Ext - Thermistor, Int - MCU


## Infobildschirm
![](http://i.imgur.com/2QoKfkX.png)

Zeigt eine Kurzübersicht von Hardwareinformationen sowie einige Statistiken.

### Danksagungen
     * TBXin - für NFE Products, Ideen und Tests
     * Zinger - für Graphiken, Ideen und Tests
     * ClockSelect - für das großartige myevic

# Disclaimer:
Es besteht keinerlei Gewährleistung für das Programm, soweit dies gesetzlich zulässig ist. Sofern nicht anderweitig schriftlich bestätigt, stellen die Urheberrechtsinhaber und/oder Dritte das Programm so zur Verfügung, „wie es ist“, ohne irgendeine Gewährleistung, weder ausdrücklich noch implizit, einschließlich – aber nicht begrenzt auf – die implizite Gewährleistung der Marktreife oder der Verwendbarkeit für einen bestimmten Zweck. Das volle Risiko bezüglich Qualität und Leistungsfähigkeit des Programms liegt bei Ihnen.

# Spenden:
Wenn das Projekt gefällt oder Sie die Entwickler unterstützen wollen, können unter [Spenden](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=ZLFDYGBRXQJGE) Spenden abgegeben werden.
