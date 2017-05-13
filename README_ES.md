# ArcticFox
*[NFE Team](http://nfeteam.org) presenta un firmware personalizado para mods de Joyetech, Wismec y Eleaf.*

```
```

**Usa [NFE Toolbox](https://github.com/TBXin/NFirmwareEditor/releases) para [instalar](https://github.com/maelstrom2001/ArcticFox/wiki/How-to-install) el firmware y configurar tu mod.**

## Lista de dispositivos compatibles:
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

## Limitaciones
Usar nuestro software de forma segura es uno de nuestros objetivos principales. Mantenemos todas las restricciones de fábrica, porque el fabricante no las ha puesto "por gusto".
¿Cuáles son las limitaciones?
* Resistencia mínima (para todos los dispositivos soportados)
  * 0.05 Ohm para el modo de control de temperatura.
  * 0.1 Ohm para el modo de vataje variable.
* Salida de vatios (depende del dispositivo)
* Corriente máxima de carga (depende del dispositivo)
* Corriente máxima de salida (depende del dispositivo)
* Rango de voltaje de salida (depende del dispositivo)

"Depende del dispositivo" significa que cada dispositivo tiene sus propios valores, elegidos por el fabricante. Puedes encontrar estos valores en la página del fabricante..

**Todas las peticiones para cambiar estos valores serán rechazadas porque no queremos que te hagas daño o estropees el dispositivo.**


## Perfiles
La principal diferencia es el perfil basado en la interfaz de usuario, es decir, estilo DNA y mayormente enforcarnos en personalizarlo más que el firmware original de Joyetech.
El perfil es el conjunto de ajustes utilizados en el atomizador, como el material, la resistencia, potencia y temperatura.
El usuario tiene 8 perfiles que pueden ser editados con NFE Toolbox, con posibilidad de asignarlos a cada uno tus atomizadores favoritos.

![](http://i.imgur.com/GF9vAbN.gif) ![](http://i.imgur.com/n7IAwpv.gif)

Los perfiles pueden cambiar automáticamente basándose en la resistencia guardada o manualmente. Para utilizar el modo automático simplemente necesitas habilitar el modo "Smart", instalar el atomizador y asignarlo al perfil que prefieras.

![](http://i.imgur.com/J8TXMpU.png) ![](http://i.imgur.com/PvMv2at.png)

Más tarde cuando vuelvas a poner el atomizador, el perfil asignado se activará automáticamente.
Si la resistencia instalada no se encuentra en tus perfiles, se te pedirá que elijas un nuevo perfil o reasignes uno existente.

Cuando cambias manualmente de perfil y el valor de la resistencia no coincide, se te pedirá que actualices los ajustes o los dejes como están.

![](http://i.imgur.com/2u0Jgwb.png) ![](http://i.imgur.com/prrhsrr.png)


## Pantalla principal

![](http://i.imgur.com/ARKJkRS.gif)

Editar la pantalla principal difere de los firmwares originales de Joyetech. Para editar las secciones en lapantalla principal, debes habilitar la opción de "edición" (por defecto, pulsando el botón de calada 4 veces). Una pulsación simple saltará a la próxima sección editable. Edita la sección seleccionada pulsando los botones de subida y bajada habituales. Para salir  del menú "edición" pulsa el botón de calada 1 segundo.


## Menú principal

(Por defecto) pulsa el botón de calada y "-" durante 1 segundo para entrar al menú.

![](http://i.imgur.com/feb0TFy.png)

### Menú de perfiles

![](http://i.imgur.com/k5lilx4.png) ![](http://i.imgur.com/5ZPdPL1.png) ![](http://i.imgur.com/eVM4jxZ.png) ![](http://i.imgur.com/6874bnH.png)

* **Wire** - material de la resistencia, si tiene control de temperatura o no (Vataje variable), puede ser estándar o definido por el usuario;
* **Coil** - resistencia guardada;
* **TCR** - puede ser editado cuando usas un Joyetech TC con TCR personalizado;
* **T. Dom** - estilo de regulación de temperatura;
* **Preheat** - control de potencia, precalentamiento o curva de potencia;
* **PI-Reg** - regulador PI para el modo TC, improves power and temperature stabilization mejora la potencia y la estabilización de temperatura:
     - PI-Reg On/Off - alterna entre el modo por defecto de Joyetech o regulación PI;
     - Range - 0..100% - rango de temperatura cuando utilizas la regulación PI. 0 significa que la regulación está siempre encendida y la distribución del control de potencia empieza con la calada, 20% por ejemplo - el regulador PI se activa cuando la temperatura de la resistencia alcanza el 20% de los valores ajustados en el perfil;
     - P - constante proporcional, cuando más alta es, más intenta se vuelve la potencia;
     - I - constante integral, cuando más alta es, la distribución de potencia es más suave.

### Menú de pantalla

![](http://i.imgur.com/ANnqWiG.png) ![](http://i.imgur.com/Z5ygFZR.png) ![](http://i.imgur.com/IKs6AeP.png) ![](http://i.imgur.com/u2wvplG.png) ![](http://i.imgur.com/f4pXIRN.png) ![](http://i.imgur.com/ozrsc7q.png)

* **Wake <>** - enciende el mod pulsando los botones habituales;
* **Logo** - muestra el logo en la pantalla principal;
* **Clock**
     - **Type** - analógico o digital;
     - **On Main** - muestra el reloj en la pantalla principal;
     - **Saver** - muestra el reloj en el modo de ahorro de energía;
* **Timeouts**
     - **Dim** - tiempo de espera hasta apagar la pantalla;
     - **Dim** :lock: - tiempo de espera hasta apagar la pantalla en modo bloqueado;
     - **Logo** - tiempo en espera hasta mostrar el logo;
     - **Clock** - tiempo en espera hasta mostrar el reloj;
* **Charge**
     - **Type** - tipo de carga en pantalla, estándar o con información adicional;
     - **Add.** - añadir sección adicional, reloj o logo;
* **Stealth** - ajustes en pantalla para el modo Stealth:
     - **Charge** - la pantalla de carga se mostrará en el modo Stealth;
     - **Saver** - el salvapantalla se mostrará en el modo Stealth;
     - **ClkOnF** - cuando el reloj está activado en la pantalla principal, se moestrará inmediatamente con una pulsación de calada simple;
* **Contrast** - ajusta el contraste/brillo de la pantalla;
* **Skin** - cambia el estilo de la pantalla principal.

### Menú de ajustes

![](http://i.imgur.com/iWCQH2q.png) ![](http://i.imgur.com/mQYC7Vi.png) ![](http://i.imgur.com/24Oqlur.png) ![](http://i.imgur.com/mS1hiZY.png)

* **1 Watt** - incremento/decremento de la potencia en 1 vátio;
* **Clicks** - acciones asignadas a
     * **2/3/4 Fire button clicks**:
          - None;
          - Edit Main - acción principal de Joyetech con 3 pulsaciones;
          - Main Menu - entrar al menú principal, igual que pulsar calada y + ;
          - Preheat - ajustes de precalentamiento del perfil activo;
          - Profiles - selector de perfiles;
          - Edit Profile - entrar en el menú de perfiles;
          - T. Dom - temperatura dominante encendida/apagada;
          - Clock - mostrar/esconder el reloj en la pantalla principal;
          - Info - mostrar información en pantalla;
          - Reset Cnt. - mostrar las estadísticas de vapeo con posibilidad de reseteo;
          - Power Bank - cambiar al modo Power Bank;
          - Coil Lock - bloquear resistencia (modos TC);
          - Key Lock - bloquear botones encendido/apagado;
          - Stealth - cambiar a modo Stealth encendido/apagado;
          - Smart On/Off - cambiar al modo Smart encendido/apagado;
          - LSL - cambiar al modo nocturno encendido/apagado;
          - Device Lock - bloquear todos los botones dejando el mod encendido;
          - On/Off - apagar o encender mod;
     * **5 Fire button clicks**:
          - On/Off - apagar o encender mod;
          - Device Lock - bloquear todos los botones dejando el mod encendido;
* **Smart** - ajustes de cambio de perfil automático:
     - Off/On/Lazy - Lazy significa que el perfil solo cambiará cuando el cambies el atomizador con el mod encendido;
     - Range - tolerencia de la resistencia;
* **Clock** - ajustes del reloj;
     - Date/Time - ajustar fecha y hora actual;
     - Adjust Time - ajustar en saltos de 1 segundo;
     - LIRC Speed - ajustar la velocidad interna del oscilador usado en mods sin cristal externo de 32768 Hz;
* **Expert** - ajustes para usuarios avanzados:

![](http://i.imgur.com/TewKhaq.png) ![](http://i.imgur.com/t24VXIO.png) ![](http://i.imgur.com/7feR2HK.png) ![](http://i.imgur.com/KqArvHQ.png)

* **USB**
     - NoSlp - no entrar en modo reposo cuando el mod está conectado por usb - puede causar que se descarguen las baterías cuando la carga finaliza;
     - Charge - las baterías se cargan cuando el mod está conectado por usb - solo para mods de varias baterías;
* **BVO** - offset del voltaje de baterías;
* **BATT** - perfil de descarga de batería;
* **SHUNT** - corrección del medidor de ohmnios;
* **ChkTCR** - check coil material TCR, revisar el material de la resistencia TCR, desactivando esta opción elimina el error TCR en resistencias grandes;
* **RCOBC** - resetea las estadísticas al cambiar las baterías;
* **RTC** - modo de reloj en tiempo real:
     - LXT - soporte de hardware completo;
     - LIRC - oscilador secundario impreciso;
     - LSL - modo software. Gasta más batería en modo reposo, pero proporciona resultados más precisos en mods sin implementación RTC;  
     ***Nota***: después de cambiar el modo RTC desconecta el usb y reinicia el mod quitando las baterías durante 30 segundos.
* **TEMP** - sensor de temperatura , Ext - thermistor, Int - MCU;
* **D. Sleep** - modo sueño profundo (se activa después de 3 minutos de actividad)::
     - Std - modo estándar;
     - Power / Lock - apaga / o bloquea el mod antes de entrar en modo sueño profundo.

### Power Bank

![](http://i.imgur.com/IxyXhex.png) ![](http://i.imgur.com/pnfnHQ0.gif) ![](http://i.imgur.com/D8dLPZJ.gif)

Soporte para adaptador Avatar RC o similar. Permite cargar dispositivos con un voltaje de 5v y hasta 2.1 amperios. Para empezar a cargar, pon el adaptador RC en el mod, conecta el dispositivo y pulsa el botón de calada. El modo Power Bank se desactiva automáticamente cuando el consumo de corriente no supera los 50mA (indicado por el mensaje "Encendido" parpadeando). Para parar la carga, pulsa el botón de calada.
Para salir del modo Power Bank mantén presionado el botón de calada o los botones de regulación a la vez.


### Pantalla de estadísticas

![](http://i.imgur.com/bsXlfpV.png) ![](http://i.imgur.com/5FG1OD6.gif)

Muestra información breve sobre el hardware y algunas estadísticas.

### Muchas gracias a:

* **TBXin** - for NFE Products and joint development
* **Zinger** - for graphics, ideas and tests
* **ArionWT** - for graphics, ideas and tests
* **ClockSelect** - for great project called myevic

# AVISO IMPORTANTE:

Este firmware es distribuido con la esperanza de que sea útil, pero sin ninguna garantía. Se proporciona "tal cual" sin garantía de ningún tipo, ya sea expresa o implícita, incluyendo, pero no limitado a, las garantías implícitas de comerciabilidad y adecuación a un propósito particular. Todo el riesgo en cuanto a la calidad y el rendimiento del firmware depende de ti.

# Donaciones:
Si te gusta nuestro proyecto y quieres ayudar a su desarrollo, puedes [donarnos](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=ZLFDYGBRXQJGE) cualquier cantidad de dinero que consideres aceptable.
