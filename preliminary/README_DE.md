##VORLÄUFIG

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
* eVic Primo
* eVic Primo 2.0
* eVic Primo Mini
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
* Predator 228
* VF Lite
* VF Stout
* VF Classic
* BV Centurion
* La Petite Box
* VS Switchbox

### Eleaf:
* Aster
* iStick Pico 75W
* iStick Pico Mega 80W
* iStick Pico Dual
* iStick Pico RDTA
* iStick iPower 80W
* iStick TC100W
* iStick TC200W
* iStick QC 200W

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

![](http://i.imgur.com/GF9vAbN.gif) ![](http://i.imgur.com/n7IAwpv.gif)

Profile können entweder automatisch gewechselt werden, in Abhängigkeit des Widerstands der Wicklung, oder manuell. Um das automatische Wechseln des Profils zu nutzen muss lediglich der "Smart" Modus aktiviert, ein Verdampfer aufgeschraubt und das gewünschte Profil ausgewählt und damit dem Verdampfer zugewiesen werden.

![](http://i.imgur.com/J8TXMpU.png) ![](http://i.imgur.com/PvMv2at.png)

Beim nächsten Aufschrauben dieses Verdampfers wird das eingestellte Profil automatisch aktiviert.
Wird der Widerstand des Verdampfers nicht in den Profilen gefunden, wird der Benutzer aufgefordert ein neues Profil zu erstellen oder ein existierendes zuzuweisen.

Bei einem manuellen Profilwechsel mit abweichenden, gespeicherten Widerständen, wird der Benutzer aufgefordert ein Profil zu aktualisieren oder die Werte des aktiven Profils beizubehalten.

![](http://i.imgur.com/2u0Jgwb.png) ![](http://i.imgur.com/prrhsrr.png)

## Hauptbildschirm

![](http://i.imgur.com/ARKJkRS.gif)

Bearbeiten des Hauptbildschirms weicht von der orignalen Joyetechfirmware ab. Zum Bearbeiten des Hauptbildschirms muss die "Edit Main" Aktion (standardmäßig 4 Feuertaster-Klicks) ausgeführt werden. Einzelndes Betätigens des Feuertasters wählt das nächste editierbare Element aus. Das ausgewählte Element wird mit den Plus- und Minustasten bearbetiet. Halten des Feuertasters für eine Sekunde verlässt den Bearbeitungsmodus.


## Hauptmenü

Gleichzeitiges Betätigen des Feuertasters und der Plus-Taste für eine Sekunde öffnet das Hauptmenü:

![](http://i.imgur.com/feb0TFy.png)

## Profilmenü

![](http://i.imgur.com/k5lilx4.png) ![](http://i.imgur.com/5ZPdPL1.png) ![](http://i.imgur.com/eVM4jxZ.png) ![](http://i.imgur.com/6874bnH.png)

* **Wire** - Drahtmaterial, Temperaturabhängig oder nicht (VW), entweder Standard oder eigene TFR-Werte;
* **Coil** - Gespeicherter Widerstand;
* **TCR** - Werte können bearbeitet werden, wenn der Joyetech TC Algorithmus mit eigener TCR ausgewählt ist;
* **T. Dom** - Temperatur-dominante Regulierung;
* **Preheat** - Leistungskontrolle, entweder Preheat oder Leistungskurve;
* **PI-Reg** - PI Regulator für TC Modus, verbesserte, stabilisierte Leistungs- und Temperaturregulierung:
     - PI-Reg On/Off - Wechsel zwischen Joyetech TC Algorithmus und PI Regulierung;
     - Range - 0..100% - Temperaturbereich in dem PI Regulierung aktiv ist. 0 bedeutet, der Regulator ist immer aktiv und kontrolliert die Leistungsabgabe von Beginn des Zuges. 20% bedeutet:PI Regulator wird aktiv wenn 20% der im Profil eingestellten Temperatur erreicht werden;
     - P - proportionale Konstante, je größer, desto drastischer die Leistungsänderung;
     - I - integrale Konstante, je größer, desto gleichmäßiger ist die Leistungsregelung.

## Screenmenü

![](http://i.imgur.com/ANnqWiG.png) ![](http://i.imgur.com/Z5ygFZR.png) ![](http://i.imgur.com/IKs6AeP.png) ![](http://i.imgur.com/u2wvplG.png) ![](http://i.imgur.com/f4pXIRN.png) ![](http://i.imgur.com/ozrsc7q.png)

* **Wake <>** - Einstellung ob Plus- und Minustaste das Display aufwecken;
* **Logo** - Logo auf dem Hauptbildschirm anzeigen;
* **Clock** - Einstellungen zur Uhr:
     - Type - Analog oder Digital;
     - On Main - Uhr auf dem Hauptbildschirm anzeigen;
     - Saver - Uhr im Standbymodus anzeigen;
* **Timeouts**
     - **Dim** - Zeit bis zum Abdunkeln des Displays;
     - **Dim** :lock: - Zeit bis zum Abdunkeln des Displays in gesperrtem Modus;
     - **Logo** - Zeit bevor das Logo angezeigt wird;
     - **Clock** - Zeit bevor die Uhr angezeigt wird;    
* **Charge** - Anzeigen von zusätzlichen Informationen auf dem Ladebildschirm, Batteriespannung(en) und Temperatur des Boards;
     - **Type** - Auswahl des Ladescreens, Standard oder mit zusätzlichen Informationen;
     - **Add.** - Zusatzelement, Uhr oder Logo;
* **Stealth** - Bildschirmeinstellungen im "Stealth" Modus:
     - **Charge** - Ladebildschirm wird im "Stealth" Modus angezeigt;
     - **Saver** - Bildschirmschoner wird im "Stealth" Modus angezeigt;
     - **ClkOnF** - wenn die Uhr im Hauptbildschirm aktiviert ist, wird die Uhr mit einzelmen Druck auf den Feuertaster angezeigt;
* **Contrast** - Helligkeit des Displays justieren;
* **Skin** - Stil des Hauptbildschirms wechseln.

## Einstellungen/Settings

![](http://i.imgur.com/iWCQH2q.png) ![](http://i.imgur.com/mQYC7Vi.png) ![](http://i.imgur.com/24Oqlur.png) ![](http://i.imgur.com/mS1hiZY.png)

* **1 Watt** - Leistung in 1Wattschritten ändern;
* **Clicks** - Aktionen, die auf folgenden Klicks liegen:
    * **2/3/4 Feuertaster-Klicks**:
      - None; - Keine
      - Edit Main - Joyetech reguläre 3-Klick Aktion;
      - Profiles - Profilauswahl;
      - T. Dom - Temperatur-dominant Regulierung an/aus;
      - Clock - Zeige/Verstecke Uhr im Hauptbildschirm;
      - On/Off - Akkuträger ein/ausschalten;
      - LSL - "Light Sleep Mode" aktivieren/deaktivieren; 
      - Main Menu - Hauptmenü öffnen, wie Feuer- und Plustaste betätigen;
      - Preheat - Preheateinstellungen des aktiven Profils;
      - Edit Profile - Profilmenü öffnen;
      - Smart On/Off - Smartmodus ein/aus
      - Info - Infobildschirm anzeigen
      - Reset Cnt. - Statistiken anzeigen, mit Möglichkeit zum Zurücksetzen jener
      - Stealth - "Stealth" Modus an/aus
      - Key Lock - Tastensperre ein/aus;
      - Coil Lock - Sperren des Wicklungswiderstand in TC-Modus an/aus;
      - Power Bank - Wechseln zu Powerbank-Modus;
    * **5 Feuertaster-Klick**:
      - On/Off - Akkuträger ein-/ausschalten;
      - Lock - Alle Tasten sperren, aber Akkuträger nicht ausschalten;
* **Smart** - Einstellungen zur automatischen Profilauswahl:
     - On/Off/Lazy; - Verhalten der automatischen Profilauswahl, "Lazy" - Profile werden bei Verdampferwechsel nur automatisch gewechselt, wenn der Akkuträger aktiv ist;
     - Range; - Toleranzbereich zur Profilauswahl durch Widerstand
* **Clock** - RTC (Realtime Clock) Einstellungen;
     - Date/Time - Zeit und Datum einstellen;
     - Adjust Time - Feinjustierung der Zeit, 1-Sekundenschritte;
     - LIRC Speed - Anpassung des internen, ungenauen Oszillators, benötigt bei Akkuträgern ohne 32768 Hz Kristal;
* **Expert** - Einstellungen für fortgeschrittene Benutzer:

![](http://i.imgur.com/TewKhaq.png) ![](http://i.imgur.com/t24VXIO.png) ![](http://i.imgur.com/7feR2HK.png) ![](http://i.imgur.com/KqArvHQ.png)

* **USB**
     - NoSlp - Bei USB-Verbindung nicht in den Schlafmodus wechseln - kann bei Akkuträgern mit mehr als einer Batterie zu Selbstentladung nach Ladevorgang führen;
     - Charge - Aufladen über USB-Verbindung aktivieren/deaktivieren - für Akkuträger mit mehr als einer Batterie;
* **BVO** - Batteriespannungskorrektur;
* **BATT** - Entladeprofil für Batterie;
* **SHUNT** - Ohm-meter Korrektur;
* **ChkTCR** - Prüfen der Draht-TCR, Ausschalten kann TCR Error bei großen Coils umgehen;
* **RCOBC** - Puff Counter bei Batteriewechsel zurücksetzen, Zurücksetzen der Vaping Statistiken;
* **RTC** - Realtime Clock Modus:
    - LXT - RTC Modul verwendet zusätzlichen 32768 Hz Oszillator, falls vorhanden;
    - LIRC - unpräzisen Oszillator verwenden
    - LSL - Light Sleep Mode, für Akkuträger ohne zusätzlichen Oszillator, hält Uhr genau, benötigt etwas mehr Energie im Ruhezustand, daher wird der User durch ein ! rechts der Batterieanzeige gewarnt;
* **TEMP** - Boardtemperatursensor, Ext - Thermistor, Int - MCU
* **D. Sleep** - Tiefschlafmodus (nach 3 Minuten Inaktivität):
     - Std - Standard Tiefschlaf;
     - Power / Lock - Schaltet den Akkuträger aus oder sperrt ihn, abhängig von der 5-Klick Einstellung.

### Powerbankmodus

![](http://i.imgur.com/IxyXhex.png) ![](http://i.imgur.com/pnfnHQ0.gif) ![](http://i.imgur.com/D8dLPZJ.gif)

Unterstützung für Avatar RC Adapter und ähnliche. Ermöglicht das Aufladen von Geräten mit einer Spannung von 5V und einer Stromstärke bis zu 2.1A . Zum Laden den RC Adapter auf den Akkuträger aufschrauben, das zu ladende Gerät verbinden und den Feuertaster einmal betätigen. Der Powerbank Modus wird automatisch abgeschaltet, wenn nicht mehr als 50 mA (ersichtlich durch Blinken von "On") abgenommen werden. Manuelles Deaktiveren der Ladung erfolgt durch einfaches Betätigen des Feuertasters.
Zum Verlassen des Powerbankmodus muss der Feuertaster gedrückt und gehalten werden oder gleichzeitig die Plus- und Minustasten gedrückt werden.


## Infobildschirm
![](http://i.imgur.com/bsXlfpV.png) ![](http://i.imgur.com/5FG1OD6.gif)

Zeigt eine Kurzübersicht von Hardwareinformationen sowie einige Statistiken.

### Danksagungen
* **TBXin** - für NFE Products und Zusammenarbeit
* **Zinger** - für Graphiken, Ideen und Tests
* **ArionWT** - für Graphiken, Ideen und Tests
* **ClockSelect** - für das großartige Projekt myevic

# Disclaimer:
Es besteht keinerlei Gewährleistung für das Programm, soweit dies gesetzlich zulässig ist. Sofern nicht anderweitig schriftlich bestätigt, stellen die Urheberrechtsinhaber und/oder Dritte das Programm so zur Verfügung, „wie es ist“, ohne irgendeine Gewährleistung, weder ausdrücklich noch implizit, einschließlich – aber nicht begrenzt auf – die implizite Gewährleistung der Marktreife oder der Verwendbarkeit für einen bestimmten Zweck. Das volle Risiko bezüglich Qualität und Leistungsfähigkeit des Programms liegt bei Ihnen.

# Spenden:
Wenn das Projekt gefällt oder Sie die Entwickler unterstützen wollen, können unter [donate](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=ZLFDYGBRXQJGE) Spenden abgegeben werden können..
