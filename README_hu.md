# ArcticFox
*Az [NFE Team](http://nfeteam.org) egyedi firmware-e Joyetech, Wismec and Eleaf modokhoz*

![](http://i.imgur.com/JP4KC8A.png)
![](http://i.imgur.com/E1e7cs1.png)

![](http://i.imgur.com/kYJcp6I.png)
![](http://i.imgur.com/TnqNYK1.png)
![](http://i.imgur.com/0XTV9xD.png)

**A firmware az [NFE Toolbox](https://github.com/TBXin/NFirmwareEditor/releases) segítségével [tölthetõ fel](https://github.com/maelstrom2001/ArcticFox/wiki/How-to-install) a modra és konfigurálható.**

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
A fõ különbség az eredeti Joyetech firmware-hez képest, hogy a felhasználói felület a DNA-hoz hasonlóan profil alapú és nagyobb hangsúly került a testreszabhatóságra.
A profil a kazán különbözõ paramétereinek együttese, mint a tekercs anyaga, ellenállása, teljesítmény és hõmérséklet adatok.
8 különbözõ profil áll rendelkezésre, melyek a NFE Toolbox segítségével hozhatók létre és szerkeszthetõk, a kedvenc kazánjainkhoz szabva.

![](http://i.imgur.com/UjtY7Ir.png)

A profilok a tekercs ellenállása alapján automatikusan vagy manuálisan válthatók. Az automatikus átkapcsolás használatához csak a "Smart" módot kell engedélyezni, majd csatlakoztatni a kazánt és hozzárendelni a kívánt profilhoz.

![](http://i.imgur.com/fadryzQ.png)

Ha késõbb ezt a kazánt tekerjük a modra, a hozzárendelt profil automatikusan aktiválódik.
Ha a csatlakoztatott kazán ellenállásához nem található korábban hozzárendelt profil, létre kell hoznunk egy újat, vagy hozzárendelhetjük egy már meglévõ profilhoz.
Ha manuálisan váltunk egy olyan profilra, amely már rendelkezik korábban mentett ellenállással, de nem passzol az aktuálisan használt kazánhoz, lehetõségünk van frissíteni a profilt, vagy megtartani a korábbi értéket.

## Main Menu

Tartsd nyomva a tûz és a plusz gombot 1 másodpercig a menübe való belépéshez

![](http://i.imgur.com/XSWOLDJ.png)

## Profile Menu

![](http://i.imgur.com/HOO0KiF.png) ![](http://i.imgur.com/2UPcLHy.png) ![](http://i.imgur.com/yNH5crk.png) ![](http://i.imgur.com/kc0PYf7.png) ![](http://i.imgur.com/CNzn7vQ.png) ![](http://i.imgur.com/3MHoldt.png)

* **Wire** - huzal anyaga, TC vagy sem (VW), beállítható standard vagy felhasználó által létrehozott TFR görbe;
* **Coil** - mentett ellenállás;
* **TCR** - az érték szerkeszthetõ, ha a Joyetech TC algoritmus van kiválasztva egyedi TCR-rel;
* **T. Dom** - hõmérséklet domináns beállítás, TC esetén a fõképernyõn egybõl a hõmérséklet állítható be;
* **Preheat** - elõfûtés VW módhoz, használható egyszerû érték vagy teljesítménygörbe;
* **PI-Reg** - PI szabályzó TC-hez, javítja a teljesítmény és a hõmérséklet stabilitását (helyes beállítás esetén):
     - PI-Reg On/Off - váltás az eredeti Joyetech és a PI szabályzás között;
     - Range - 0..100% - az a hõmérsékletsáv, ahol a PI szabályzó aktív. Ha a beállított érték 0, a szabályzó mindig aktív, ha az érték például 20%, a PI szabályzás akkor kapcsol be, ha a tekercs hõmérséklete elérte a profilban beállított érték 20%-át;
     - P - proporcionális (arányos) tag, minél nagyobb, annál nagyobb a teljesítményváltozás, érzékenyebb a szabályzó. Túl nagy érték esetén a szabályzás instabillá válhat.;
     - I - integráló tag, minél nagyobb, annál simább, annál kevésbé hullámzó a teljesítmény. Érdemes figyelni a túllövésre.

## Screen Menu

![](http://i.imgur.com/6jddZL9.png) ![](http://i.imgur.com/3fRgkGN.png) ![](http://i.imgur.com/FmVjNro.png) ![](http://i.imgur.com/2UYldpC.png)

* **Dim** - mennyi idõ alatt halványodjon el a kijelzõ;
* **Wake <>** - mod felébresztés +/- gombokkal;
* **Charge** - mutasson plusz információt töltés közben, cellafeszültség, panel hõmérséklete;
* **Logo** - mutassa a logót a fõképernyõn;
* **Clock** - óra beállításai:
     - Type - analóg vagy digitális;
     - On Main - mutassa az órát a fõképernyõn;
     - Saver - mutassa az órát standby módban;
* **Selector** - mutasson plusz profil információkat a "Select Profile" képernyõn;
* **Contrast** - kijelzõ fényerejének változtatása;
* **Skin** - fõképernyõ stílusának megváltoztatása.

## Settings Menu

![](http://i.imgur.com/aDuSk3n.png) ![](http://i.imgur.com/3JeWUqf.png) ![](http://i.imgur.com/8V1VCeo.png)

* **1 Watt** - teljesítmény változtatása 1 Wattal;
* **Menu** - New - profilváltás a +/- gombok használatával, Old - váltás "Edit Main" gombnyomással (3x tûz);
* **Smart** - automatikus profilváltás beállítása:
     - On/Off;
     - ellenállás tolerancia;
     - mutassa a profil menüt új hozzárendelés esetén;
* **Clicks** - 2/3/4 tûzgombnyomáshoz rendelhetõ mûveletek:
     - semmi;
     - Edit Main - a Joyetech eredeti beállítása 3x tûzgombnyomásra;
     - Profiles - profilválasztó;
     - T. Dom - hõmérséklet domináns mód ki/be kapcsolása;
     - Clock - mutassa/rejtse el az órát a fõképernyõn;
     - On/Off - mod ki/be kapcsolása;
     - LSL - "light sleep" mód ki/be kapcsolása;
     - Main Menu - belépés a fõmenübe, mint a tûz/+ gombkombinációval;
     - Preheat - aktuális profil elõfûtésének beállítása;
     - Edit Profile - belépés a profil menübe;
     - Smart On/Off;
     - Mutassa az info képernyõt.
* **RTC** - realtime clock beállítása;
* **Expert** - beállítások haladó felhasználóknak:

![](http://i.imgur.com/UZBrHjJ.png) ![](http://i.imgur.com/7fT0pNi.png) ![](http://i.imgur.com/edejq3z.png) ![](http://i.imgur.com/FoH1vaE.png)

* **USB**
     - NoSlp - ne lépjen mély sleep módba, USB csatlakozás esetén;
     - Charge - az eszköz töltse az akkumulátort, miközben USB-n csatlakozik;
* **BVO** - cellafeszültség offset;
* **BATT** - cellakisülési profil;
* **SHUNT** - ellenállásmérés korrekciója;
* **ChkTCR** - ellenõrizze a tekercs anyagának TCR értékét, az opciót kikapcsolva vastag huzal, nagy fémtömeg esetén megszûnik a "TCR error" hibaüzenet;
* **RCOBC** - számlálók resetelése akkucsere esetén, törli a használati statisztikákat;
* **X32** - RTC modul használja a másodlagos 32768 Hz-es oszcillátort, ha van ilyen a modban;
* **LSL** - Light Sleep Mode, másodlagos oszcillátorral nem rendelkezõ készülékek esetén pontosabb RTC. Némi energiát vesz igénybe standby módban ezért ! figyelmezteti a felhasználót az akkumulátor kijelzõ mellett;
* **TEMP** - panel hõmérsékleti szenzor, Ext - thermistor, Int - MCU


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
