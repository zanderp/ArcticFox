# ArcticFox
*[NFE Team](http://nfeteam.org) va prezinta Firmware custom pentru Joyetech, Wismec si Eleaf battery mods*

![](http://i.imgur.com/PqSrmLb.png) ![](http://i.imgur.com/C8Lu9SG.png) ![](http://i.imgur.com/aBhNKxV.png) ![](http://i.imgur.com/rk6gZo8.png) ![](http://i.imgur.com/5mU3FAB.png) ![](http://i.imgur.com/wl8wR8d.png) ![](http://i.imgur.com/s3yNIEf.png)

**Folositi [NFE Toolbox](https://github.com/TBXin/NFirmwareEditor/releases) pentru [instalare](https://github.com/maelstrom2001/ArcticFox/wiki/How-to-install) firmware si configurare a dispozitivului.**

## Lista de dispozitive suportate:
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

## Limitari
Utilizarea sigura a acestui softare este una din prioritatile noastre. Noi pastram toate restrictiile din fabrica pentru ca producatorii acestor dispozitive NU le-au pus de pomana.
Care sunt aceste limitatii/restrictii?
* Rezistenta minima (Pentru toate dispozitivele suportate)
  * 0.05 Ohm pentru modul Temperature Control(Controlul Temperaturii)
  * 0.1 Ohm pentru modul Vari-Watt
* Puterea Electrica de Iesire (Depinde de dispozitiv)
* Curentul Maxim de Incarcare (Depinde de dispozitiv)
* Curentul Maxim de iesire (Depinde de dispozitiv)
* Limita Voltajului de Iesire (Depinde de dispozitiv)

"Depinde de dispozitiv" inseamna ca fiecare dispozitiv are propriile lui valori care sunt alese de producator. Puteti gasi aceste valori pe pagina web a producatorului.

**Toate cerintele de modificare ale acestor valori vor fi ignorate deoarece noi nu dorim sa va raniti sau sa se strice dipozitivul.**


## Profilele
Diferenta majora este ca aceste profile sunt bazate pe interfata utilizatorului si sunt axate pe customizarea softului original Joyetech.
Profilul este un set de parametrii folositi de atomizor cum ar fi materialul bobinei, rezistenta, puterea si valorile temperaturii.
Utilizatorul va avea 8 profile care pot fi editate cu NFE Toolbox si care pot fi adaugate atomizoarelor favorite.

![](http://i.imgur.com/GF9vAbN.gif) ![](http://i.imgur.com/n7IAwpv.gif)

Profilele pot fi schimbate intr-un mod automat bazat pe rezistenta bobinei si modul manual. Tot ce trebuie sa faceti pentru a folosi schimbarea automata a profilelor este sa activati modulul "Smart", sa instalati atomizorul si sa ii atribuiti profilul dorit.

![](http://i.imgur.com/J8TXMpU.png) ![](http://i.imgur.com/PvMv2at.png)

Cand veti reinstala acest atomizor mai tarziu, profilul atribuit va fi activat automat.
Daca rezistenta atomizorului instalat nu este gasita in profile veti fi rugat sa selectati un profil nou sau sa atribuiti unul existent.

Cand schimbati manual profilul care a salvat rezistenta care nu exista veti fi intrebat daca doriti sa actualizati sau sa mentineti setarile profilului selectat.

![](http://i.imgur.com/2u0Jgwb.png) ![](http://i.imgur.com/prrhsrr.png)


## Ecranul Principal

![](http://i.imgur.com/ARKJkRS.gif)

Editarea ecranului principal difera de modul original al softurilor Joyetech. Pentru a edita elementele de pe ecranul principal avem o combinatie numita "Edit Main"(Apasati de 4 ori pe butonul de pornire). Apasand o singura data pe butonul de pornire va trece pe urmatorul element editabil. Editati elementul selectat apasand pe butoanele de reglaj. Pentru a iesi apasati pe butonul de pornire pentru aproximativ o secunda.


## Meniul Principal

Apasati butonul de pornire impreuna cu butonul Plus pentru aproximativ o secunda pentru a intra in meniu(setari implicite).

![](http://i.imgur.com/feb0TFy.png) ![](http://i.imgur.com/be2BWSt.png)

### Meniul Profil

![](http://i.imgur.com/k5lilx4.png) ![](http://i.imgur.com/5ZPdPL1.png) ![](http://i.imgur.com/eVM4jxZ.png) ![](http://i.imgur.com/6874bnH.png)

* **Wire(Fir)** - materialul bobinei, senzor de temperatura (VW), poate fi setat ca standard sau definit de utilizator TFR;
* **Coil(Bobina)** - valoarea salvata a rezistentei bobinei;
* **TCR** - voloare care poate fi editata cand selectati algoritmul Joyetech TC cu parametrii TCR personalizati;
* **T. Dom** - reglarea determinata de temperatura;
* **Preheat(Preincalzire)** - controlul puterii, utilizare preincalzire sau curba de putere;
* **PI-Reg** - Regulator PI pentru modul TC, imbunatateste puterea si stabilizeaza temperatura:
     - PI-Reg On/Off - comuta intre modul predefinit de Joyetech si reglarea PI;
     - Range - 0..100% - intervalul de temperatura cand reglarea PI devine activa. 0 inseamna ca reglajul este pornit si controleaza puterea de la inceput sau la vapare, 20% ca exemplu - reglajul PI se activeaza cand consumul ajunge la 20% din setarile profilului;
     - P - constanta proportionala, cu cat este mai mare, cu atat mai mare este puterea;
     - I - constanta integrala, cu cat este mai mare cu atat puterea este mai mica.

### Meniul Ecranului

![](http://i.imgur.com/ANnqWiG.png) ![](http://i.imgur.com/Z5ygFZR.png) ![](http://i.imgur.com/IKs6AeP.png) ![](http://i.imgur.com/u2wvplG.png) ![](http://i.imgur.com/f4pXIRN.png) ![](http://i.imgur.com/ozrsc7q.png)

* **Wake <>(trezilre)** - modul de trezire cand se apasa pe butoanele de reglaj;
* **Logo** - arata logo pe ecranul principal;
* **Clock(Ceas)**
     - **Type(Tip)** - analog sau digital;
     - **On Main(Pe principal)** - arata ceasul in ecranul principal;
     - **Saver** - arata ceasul cand dispozitivul este in standby;
* **Timeouts**
     - **Dim** - idle time before the screen turns off;
     - **Dim** ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - idle time before the screen turns off in locked state;
     - **Logo** - idle time before displaying logo;
     - **Clock** - idle time before displaying clock;
* **Charge**
     - **Type** - charging screen type, standard or with additional information;
     - **Add.** - extra item, clock or logo;
* **Stealth** - settings for screen in Stealth Mode:
     - **Charge** - charging screen will be shown in Stealth Mode;
     - **Saver** - screen saver will be shown in Stealth Mode;
     - **ClkOnF** - when Clock on Main Screen option is enabled, clock will be shown immediately on single Fire click;
* **Contrast** - adjust brightness of display;
* **Skin** - change main screen style.

### Settings Menu

![](http://i.imgur.com/iWCQH2q.png) ![](http://i.imgur.com/mQYC7Vi.png) ![](http://i.imgur.com/24Oqlur.png) ![](http://i.imgur.com/mS1hiZY.png)

* **1 Watt** - increment/decrement power by 1,0 Watt;
* **Clicks** - actions assigned on
     * **2/3/4 Fire button clicks**:
          - None;
          - Edit Main - Joyetech default 3-clicks action;
          - Main Menu - enter Main Menu, the same as Fire + ;
          - Preheat - preheat settings for active profile;
          - Profiles - Profiles Selector;
          - Edit Profile - enter Profile Menu;
          - T. Dom - temperature-dominant on/off;
          - Clock - show/hide clock on main screen;
          - Info - show Info Screen;
          - Reset Cnt. - show vaping stats info screen with opportunity to reset counters;
          - ![](https://cdn4.iconfinder.com/data/icons/font-awesome-2/2048/f011-16.png) Bank - switch box to Power Bank mode;
          - Coil ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - switch coil resistance lock on/off (for TC modes);
          - Key ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - switch Keylock on/off;
          - Stealth - switch Stealth Mode on/off;
          - Smart On/Off - switch Smart Mode on/off;
          - LSL - switch light sleep mode on/off;
          - Device ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - switch Device Lock on / off (lock all buttons but leave mod powered on);
          - On/Off - switch mod on/off;
     * **5 Fire button clicks**:
          - On/Off - switch mod on/off;
          - Device ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - lock all buttons but leave mod powered on;
* **Smart** - automatic switching profiles settings:
     - Off/On/Lazy - Smart Mode behavior setting, Lazy means that profile can be switched automatically only on atomizer change while the box is in active state;
     - Range - resistance tolerance;
* **Clock** - realtime clock setup;
     - Date/Time - set current date and time;
     - Adjust Time - precise adjusting time by 1 second step;
     - LIRC Speed - adjusting speed of internal imprecise oscillator used on boxes without external 32768 Hz crystal on board;
* **Expert** - settings for advanced users:

![](http://i.imgur.com/TewKhaq.png) ![](http://i.imgur.com/t24VXIO.png) ![](http://i.imgur.com/7feR2HK.png) ![](http://i.imgur.com/pp3TTaR.png)

* **USB**
     - NoSlp - do not enter deep sleep mode while connected to USB - may lead to self-discharging multi-cells boxes after charging stops;
     - Charge - device is charging batteries while connected to USB - for multi-cells boxes only;
* **BVO** - batteries voltages offset;
* **BATT** - battery discharge profile;
* **SHUNT** - Ohm-meter correction;
* **ChkTCR** - check coil material TCR, switching this option to off can eliminate TCR Error on heavy coils;
* **RCOBC** - Reset Counters on Battery Change, clear vaping statistics;
* **RTC** - Realtime Clock mode:
     - LXT - full hardware support;
     - LIRC - inaccurate secondary oscillator;
     - LSL - software mode. It takes some more energy in standby mode, but provides more accurate results on boxes without hardware RTC implementation;  
     ***Note***: after switching RTC mode unplug USB and reboot your box by pulling out batteries for about 30 sec.
* **TEMP** - board temperature sensor, Ext - thermistor, Int - MCU;
* **D. Sleep** - deep sleep (enter after 3 minutes of inactivity) mode:
     - Std - standard deep sleep;
     - ![](https://cdn4.iconfinder.com/data/icons/font-awesome-2/2048/f011-16.png) - switch box to powered off state before going into deep sleep;
     - ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - lock box before going into deep sleep.

### Power Bank

![](http://i.imgur.com/IxyXhex.png) ![](http://i.imgur.com/pnfnHQ0.gif) ![](http://i.imgur.com/D8dLPZJ.gif)

Support for Avatar RC adapter and similar. Provides charging devices with a voltage of 5 volts and current up to 2.1 amps. To start charging, put RC adapter on box, connect device and press Fire button. Power Bank mode has auto-off feature when current drain is not exceed 50 mA (indicated by blinking label "On"). To stop charging, press Fire button.
To exit Power Bank mode press and hold Fire button, or regulatory buttons simultaneously.


### Info Screen

![](http://i.imgur.com/bsXlfpV.png) ![](http://i.imgur.com/5FG1OD6.gif)

Shows brief hardware information and some stats.

### Many thanks to:

* **TBXin** - for NFE Products and joint development
* **Zinger** - for graphics, ideas and tests
* **ArionWT** - for graphics, ideas and tests
* **ClockSelect** - for great project called myevic

# Disclaimer:

The firmware is distributed in the hope that it will be useful, but without any warranty. It is provided "as is" without warranty of any kind, either expressed or implied, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose. The entire risk as to the quality and performance of the firmware is with you.

# Donations:
If you like our project and you want to help in its development, you can [donate](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=ZLFDYGBRXQJGE) us the amount of money you deem acceptable.
