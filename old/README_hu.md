# ArcticFox
*Az [NFE Team](http://nfeteam.org) egyedi firmware-e Joyetech, Wismec and Eleaf modokhoz*

![](http://i.imgur.com/JP4KC8A.png)
![](http://i.imgur.com/E1e7cs1.png)

![](http://i.imgur.com/kYJcp6I.png)
![](http://i.imgur.com/TnqNYK1.png)
![](http://i.imgur.com/0XTV9xD.png)

**A firmware az [NFE Toolbox](https://github.com/TBXin/NFirmwareEditor/releases) segítségével [tölthető fel](https://github.com/maelstrom2001/ArcticFox/wiki/How-to-install) a modra és konfigurálható.**

## Támogatott eszközök:
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

## Profiles
A fő különbség az eredeti Joyetech firmware-hez képest, hogy a felhasználói felület a DNA-hoz hasonlóan profil alapú és nagyobb hangsúly került a testreszabhatóságra.
A profil a kazán különböző paramétereinek együttese, mint a tekercs anyaga, ellenállása, teljesítmény és hőmérséklet adatok.
8 különböző profil áll rendelkezésre, melyek a NFE Toolbox segítségével hozhatók létre és szerkeszthetők, a kedvenc kazánjainkhoz szabva.

![](http://i.imgur.com/UjtY7Ir.png)

A profilok a tekercs ellenállása alapján automatikusan vagy manuálisan válthatók. Az automatikus átkapcsolás használatához csak a "Smart" módot kell engedélyezni, majd csatlakoztatni a kazánt és hozzárendelni a kívánt profilhoz.

![](http://i.imgur.com/fadryzQ.png)

Ha később ezt a kazánt tekerjük a modra, a hozzárendelt profil automatikusan aktiválódik.
Ha a csatlakoztatott kazán ellenállásához nem található korábban hozzárendelt profil, létre kell hoznunk egy újat, vagy hozzárendelhetjük egy már meglévő profilhoz.
Ha manuálisan váltunk egy olyan profilra, amely már rendelkezik korábban mentett ellenállással, de nem passzol az aktuálisan használt kazánhoz, lehetőségünk van frissíteni a profilt, vagy megtartani a korábbi értéket.

## Main Menu

Tartsd nyomva a tűz és a plusz gombot 1 másodpercig a menübe való belépéshez

![](http://i.imgur.com/XSWOLDJ.png)

## Profile Menu

![](http://i.imgur.com/HOO0KiF.png) ![](http://i.imgur.com/2UPcLHy.png) ![](http://i.imgur.com/yNH5crk.png) ![](http://i.imgur.com/kc0PYf7.png) ![](http://i.imgur.com/CNzn7vQ.png) ![](http://i.imgur.com/3MHoldt.png)

* **Wire** - huzal anyaga, TC vagy sem (VW), beállítható standard vagy felhasználó által létrehozott TFR görbe;
* **Coil** - mentett ellenállás;
* **TCR** - az érték szerkeszthető, ha a Joyetech TC algoritmus van kiválasztva egyedi TCR-rel;
* **T. Dom** - hőmérséklet domináns beállítás, TC esetén a főképernyőn egyből a hőmérséklet állítható be;
* **Preheat** - előfűtés VW módhoz, használható egyszerű érték vagy teljesítménygörbe;
* **PI-Reg** - PI szabályzó TC-hez, javítja a teljesítmény és a hőmérséklet stabilitását (helyes beállítás esetén):
     - PI-Reg On/Off - váltás az eredeti Joyetech és a PI szabályzás között;
     - Range - 0..100% - az a hőmérsékletsáv, ahol a PI szabályzó aktív. Ha a beállított érték 0, a szabályzó mindig aktív, ha az érték például 20%, a PI szabályzás akkor kapcsol be, ha a tekercs hőmérséklete elérte a profilban beállított érték 20%-át;
     - P - proporcionális (arányos) tag, minél nagyobb, annál nagyobb a teljesítményváltozás, érzékenyebb a szabályzó. Túl nagy érték esetén a szabályzás instabillá válhat.;
     - I - integráló tag, minél nagyobb, annál simább, annál kevésbé hullámzó a teljesítmény. Érdemes figyelni a túllövésre.

## Screen Menu

![](http://i.imgur.com/6jddZL9.png) ![](http://i.imgur.com/3fRgkGN.png) ![](http://i.imgur.com/FmVjNro.png) ![](http://i.imgur.com/2UYldpC.png)

* **Dim** - mennyi idő alatt halványodjon el a kijelző;
* **Wake <>** - mod felébresztés +/- gombokkal;
* **Charge** - mutasson plusz információt töltés közben, cellafeszültség, panel hőmérséklete;
* **Logo** - mutassa a logót a főképernyőn;
* **Clock** - óra beállításai:
     - Type - analóg vagy digitális;
     - On Main - mutassa az órát a főképernyőn;
     - Saver - mutassa az órát standby módban;
* **Contrast** - kijelző fényerejének változtatása;
* **Skin** - főképernyő stílusának megváltoztatása.

## Settings Menu

![](http://i.imgur.com/aDuSk3n.png) ![](http://i.imgur.com/3JeWUqf.png) ![](http://i.imgur.com/8V1VCeo.png)

* **1 Watt** - teljesítmény változtatása 1 Wattal;
* **Menu** - New - profilváltás a +/- gombok használatával, Old - váltás "Edit Main" gombnyomással (3x tűz);
* **Smart** - automatikus profilváltás beállítása:
     - On/Off;
     - ellenállás tolerancia;
     - mutassa a profil menüt új hozzárendelés esetén;
* **Clicks** - 2/3/4 tűzgombnyomáshoz rendelhető műveletek:
     - semmi;
     - Edit Main - a Joyetech eredeti beállítása 3x tűzgombnyomásra;
     - Profiles - profilválasztó;
     - T. Dom - hőmérséklet domináns mód ki/be kapcsolása;
     - Clock - mutassa/rejtse el az órát a főképernyőn;
     - On/Off - mod ki/be kapcsolása;
     - LSL - "light sleep" mód ki/be kapcsolása;
     - Main Menu - belépés a főmenübe, mint a tűz/+ gombkombinációval;
     - Preheat - aktuális profil előfűtésének beállítása;
     - Edit Profile - belépés a profil menübe;
     - Smart On/Off;
     - Mutassa az info képernyőt.
* **RTC** - realtime clock beállítása;
* **Expert** - beállítások haladó felhasználóknak:

![](http://i.imgur.com/UZBrHjJ.png) ![](http://i.imgur.com/7fT0pNi.png) ![](http://i.imgur.com/edejq3z.png) ![](http://i.imgur.com/FoH1vaE.png)

* **USB**
     - NoSlp - ne lépjen mély sleep módba, USB csatlakozás esetén;
     - Charge - az eszköz töltse az akkumulátort, miközben USB-n csatlakozik;
* **BVO** - cellafeszültség offset;
* **BATT** - cellakisülési profil;
* **SHUNT** - ellenállásmérés korrekciója;
* **ChkTCR** - ellenőrizze a tekercs anyagának TCR értékét, az opciót kikapcsolva vastag huzal, nagy fémtömeg esetén megszűnik a "TCR error" hibaüzenet;
* **RCOBC** - számlálók resetelése akkucsere esetén, törli a használati statisztikákat;
* **X32** - RTC modul használja a másodlagos 32768 Hz-es oszcillátort, ha van ilyen a modban;
* **LSL** - Light Sleep Mode, másodlagos oszcillátorral nem rendelkező készülékek esetén pontosabb RTC. Némi energiát vesz igénybe standby módban ezért ! figyelmezteti a felhasználót az akkumulátor kijelző mellett;
* **TEMP** - panel hőmérsékleti szenzor, Ext - thermistor, Int - MCU


## Info Screen
![](http://i.imgur.com/2QoKfkX.png)

Rövid HW információ és némi statisztika.

### Köszönet:
     * TBXin - for NFE Products, ideas and tests
     * Zinger - for graphics, ideas and tests
     * ClockSelect - for great project called myevic

### Fordította:
     * balazsk

# Disclaimer:

The firmware is distributed in the hope that it will be useful, but without any warranty. It is provided "as is" without warranty of any kind, either expressed or implied, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose. The entire risk as to the quality and performance of the firmware is with you.

# Támogatás:
Ha szeretnéd támogatni a projektet, ezzel segítve a fejlesztésben, akkor itt megteheted egy általad választott összeggel: [támogatás](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=ZLFDYGBRXQJGE).
