### *Preliminary*
# ArcticFox
*[NFE Team](http://nfeteam.org) presents custom Firmware for Joyetech, Wismec and Eleaf battery mods*

```
```

**Use [NFE Toolbox](https://github.com/TBXin/NFirmwareEditor/releases) for [installing](https://github.com/maelstrom2001/ArcticFox/wiki/How-to-install) firmware and configuring your device.**

## List of supported devices:
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

## Limitations
The safe use of our software one of our main goals. We retain all factory restrictions, because the device manufacturer is not just for fun made them.
What we call limitations?
* Minimal Resistance (For all supported devices)
  * 0.05 Ohm for Temperature Control mode
  * 0.1 Ohm for Vari-Watt mode
* Output Wattage (Depending on the device)
* Maximum Charging Current (Depending on the device)
* Maximum Output Current (Depending on the device)
* Output Voltage Range (Depending on the device)

"Depending on the device" means that each device has own values, which are choosen by the manufacturer. The exact values you can find on the product page on the manufacturer's website.

**All requests to change these values will be rejected as we don't want you to hurt yourself or your device.**


## Profiles
The main difference is the profile based user interface, so to say, the DNA-style, and the larger focus on customization than original Joyetech firmware.
Profile is the set of parameters of used atomizer, such as coil material, resistance, power and temperature values.
The user have 8 profiles which can be edited with NFE Toolbox, and which can be assigned to his favourite atomizers.

```
```

Profiles can be switched automatically, based on saved coil resistance, and in manual mode. All you need to use the automatic switch is to enable "Smart" mode, install atomizer and assign them to the desired profile.

```
```

When you re-install this atomizer later, assigned profile will be activated automatically.
If resistance of installed atomizer is not found in profiles, you'll be prompted to select new profile or re-assign existing.
When you switching manually to profile that have saved resistance mismatch, you'll be prompted to update or keep settings of selected profile.


## Main Screen

![](http://i.imgur.com/ARKJkRS.gif)

Editing the main screen differs from original Joyetech firmwares. To edit items on main screen, call action "Edit Main" (4 Fire button clicks by default). Single Fire button click will switch next available editable item. Edit selected item by pressing regulatory buttons. To exit edit mode hold Fire button for about 1 sec.


## Main Menu

Hold Fire and Plus buttons (by default) for a 1 second to enter menu.

![](http://i.imgur.com/feb0TFy.png)

### Profile Menu

![](http://i.imgur.com/k5lilx4.png) ![](http://i.imgur.com/5ZPdPL1.png) ![](http://i.imgur.com/eVM4jxZ.png) ![](http://i.imgur.com/6874bnH.png)

* **Wire** - coil material, temperature sensing or not (VW), can be set to standard or user-defined TFR;
* **Coil** - saved coil resistance;
* **TCR** - value can be edited when selected Joyetech TC algo with custom TCR;
* **T. Dom** - temperature-dominant regulation style;
* **Preheat** - power control, use preheat or power curve;
* **PI-Reg** - PI Regulator for TC mode, improves power and temperature stabilization:
     - PI-Reg On/Off - switch between stock Joyetech and PI regulation;
     - Range - 0..100% - temperature range when PI regulation becomes active. 0 means that regulator is always on and controls power distribution from start of puff, 20% for example - PI regulator turns on when temperature of coil reached 20% range from profile settings;
     - P - proportional constant, the larger it is, the sharper the power changed;
     - I - integral constant, the larger it is, the settled power distribution is smoother.

### Screen Menu

![](http://i.imgur.com/ANnqWiG.png) ![](http://i.imgur.com/Z5ygFZR.png) ![](http://i.imgur.com/IKs6AeP.png) ![](http://i.imgur.com/04QP7e7.png) ![](http://i.imgur.com/f4pXIRN.png) ![](http://i.imgur.com/ozrsc7q.png)

* **Wake <>** - waking mod up by pressing regulatory buttons;
* **Logo** - show logo on main screen;
* **Clock**
     - **Type** - analog or digital;
     - **On Main** - show clock on main screen;
     - **Saver** - show clock in standby mode;
* **Timeouts**
     - **Dim** - idle time before the screen turns off;
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

![](http://i.imgur.com/Wx1jgOT.png) ![](http://i.imgur.com/mQYC7Vi.png) ![](http://i.imgur.com/24Oqlur.png) ![](http://i.imgur.com/P8IkuiY.png)

* **1 Watt** - increment/decrement power by 1,0 Watt;
* **Clicks** - actions assigned on 2/3/4/5 Fire button clicks:
     - None;
     - Edit Main - Joyetech default 3-clicks action;
     - Profiles - Profiles Selector;
     - T. Dom - temperature-dominant on/off;
     - Clock - show/hide clock on main screen;
     - On/Off - switch mod on/off;
     - LSL - switch light sleep mode on/off;
     - Main Menu - enter Main Menu, the same as Fire + ;
     - Preheat - preheat settings for active profile;
     - Edit Profile - enter Profile Menu;
     - Smart On/Off - switch Smart Mode on/off;
     - Info - show Info Screen;
     - Reset Cnt. - show vaping stats info screen with opportunity to reset counters;
     - Stealth - switch Stealth Mode on/off;
     - Key Lock - switch Keylock on/off;
     - Coil Lock - switch coil resistance lock on/off (for TC modes);
* **Smart** - automatic switching profiles settings:
     - Off/On/Lazy - Smart Mode behavior setting, Lazy means that profile can be switched automatically only on atomizer change while the box is in active state;
     - resistance tolerance;
* **RTC** - realtime clock setup;
* **Expert** - settings for advanced users:

![](http://i.imgur.com/xoWDOox.png) ![](http://i.imgur.com/t24VXIO.png) ![](http://i.imgur.com/7feR2HK.png) ![](http://i.imgur.com/xoWDOox.png)

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
* **TEMP** - board temperature sensor, Ext - thermistor, Int - MCU.


### Power Bank

```
```

Support for Avatar RC adapter and similar. Provides charging devices with a voltage of 5 volts and current up to 2.1 amps. To start charging, put RC adapter on box, connect device and press Fire button. Power Bank mode has auto-off feature when current drain is not exceed 50 mA (indicated by blinking label "On"). To stop charging, press Fire button.
To exit Power Bank mode press and hold Fire button, or regulatory buttons simultaneously.


### Info Screen

![](http://i.imgur.com/bsXlfpV.png)

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
