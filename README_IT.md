# ArcticFox
*Il [team NFE](http://nfeteam.org) presenta un custom firmware per le battery mod Joyetech, Wismec ed Eleaf*

![](http://i.imgur.com/JP4KC8A.png)
![](http://i.imgur.com/E1e7cs1.png)

![](http://i.imgur.com/kYJcp6I.png)
![](http://i.imgur.com/TnqNYK1.png)
![](http://i.imgur.com/0XTV9xD.png)

**Utilizza l'[NFE Toolbox](https://github.com/TBXin/NFirmwareEditor/releases) per [installare](https://github.com/maelstrom2001/ArcticFox/wiki/How-to-install) il firmware e per configurare il tuo dispositivo.**

## Lista delle battery mod supportate:
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

## Profili
La differenza principale è l'interfaccia utente, simile a quella DNA, pienamente modificabile rispetto al firmware originale Joyetech.
I profili sono composti da set di parametri utilizzati dall'atomizzatore come il materiale delle coil, le resistenze, potenza erogata e valori relativi alle temperature.
L'utente ha a disposizione 8 profili personalizzabili attraverso la NFE toolbox, che può assegnare liberamente al suo atomizzatore preferito.

![](http://i.imgur.com/UjtY7Ir.png)

I profili possono essere cambiati automaticamente sulla base dei dati raccolti dal firmware oppure in modalità manuale.
Per far si che il firmware utilizzi questa funzione è necessario abilitare la "Smart" mode, installare l'atomizzatore ed assegnarlo al profilo desiderato.

![](http://i.imgur.com/fadryzQ.png)

Quando reinstallerai l'atomizzatore più tardi, il profilo precedentemente assegnato verrà attivato automaticamente.
Se la resistenza dell'atomizzatore installato non viene trovato nei profili, verrà chiesto all'utente di assegnarne uno nuovo o di riassegnare un profilo esistente.
Quando l'utente cambia manualmente il profilo e la resistenza non combacia con i dati inclusi nello stesso, verrà chiesto se mantenere la precedente configurazione o aggiornarla.
## Main Menu

Per accedere al menù, premere il pulsante Fire ed il pulsante Plus per un secondo.

![](http://i.imgur.com/XSWOLDJ.png)

## Profile Menu

![](http://i.imgur.com/HOO0KiF.png) ![](http://i.imgur.com/2UPcLHy.png) ![](http://i.imgur.com/yNH5crk.png) ![](http://i.imgur.com/kc0PYf7.png) ![](http://i.imgur.com/CNzn7vQ.png) ![](http://i.imgur.com/3MHoldt.png)

* **Wire** - materiale bobina, le modalità temperature control  o non (VW), possono essere impostate in modalità standard oppure definite dall'utente con valori TFR;
* **Coil** - resistenza salvata;
* **TCR** - il valore TC Joyetech può essere modificato con un valore TCR personalizzato;
* **T. Dom** - stile di regolazione temperature-dominant ;
* **Preheat** - controllo della potenza, utilizza il preriscaldamento o la curva di potenza;
* **PI-Reg** - Regolatore PI  per la modalità TC, migliora la potenza e la stabilizzazione della temperatura;
     - PI-Reg On/Off - Modifica la modalità selezionata tra quella standard Joytech e quella che regola il PI;
     - Range - 0..100% - Regola il range della temperatura quando la modalità PI è attiva. 0 corrisponde alla suddetta modalità sempre attiva e  controlla la distribuzione della potenza dall'inizio della svapata, 20% per esempio -  il regolatore PI si attiva quando la temperatura della coil raggiunge il range del 20% dai settaggi definiti nel profilo;
     - P - costante proporzionale, più larga è più è nitido il cambiamento di potenza; 
     - I - costante integrale, più larga è  più la distribuzione della potenza è stabile.

## Screen Menu

![](http://i.imgur.com/6jddZL9.png) ![](http://i.imgur.com/3fRgkGN.png) ![](http://i.imgur.com/FmVjNro.png) ![](http://i.imgur.com/2UYldpC.png)

* **Dim** - timeout del display;
* **Wake <>** - risveglia la mod premendo i pulsanti regolatori;
* **Charge** - mostra informazioni accessorie sulla schermata di caricamento, voltaggi della batteria e temperatra del circuito;
* **Logo** - mostra il logo sulla schermata principale;
* **Clock** - mostra l'orologio sullo schermo:
     - Type - analogico o digitale;
     - On Main - mostra l'orologio sulla schermata principale;
     - Saver - mostra l'orologio sullo screensaver;
* **Contrast** - modifica la luminosità dello schermo;
* **Skin** - cambia la skin .

## Settings Menu

![](http://i.imgur.com/aDuSk3n.png) ![](http://i.imgur.com/3JeWUqf.png) ![](http://i.imgur.com/8V1VCeo.png)

* **1 Watt** - incrementa/decrementa la potenza di 1,0 Watt;
* **Menu** - New - scorri i profili utilizzando i pulsanti selettori, Old - scorrendoli attraverso l'azione standard "Edit Main"
* **Smart** - cambiamento automatico dei settaggi per i profili;
     - On/Off;
     - tolleranza resistenza;
     - mostra il Profile Menu dopo averne assegnato uno nuovo;
* **Clicks** - assegna un azione alle pressioni ripetute del pulsante Fire:
     - None; (nessuna azione assegnata)
     - Edit Main - (modifiche principali) azione di default del firmware originale Joytech, a tre pressioni consecutive;
     - Profiles - Selettore profili;
     - T. Dom - temperatura dominante on/off;
     - Clock - mostra/nascondi l'orologio sullo schermata principale;
     - On/Off - attiva/disattiva la modalità;
     - LSL - Attiva/disattiva la light sleep mode;
     - Main Menu - entra nel menù principale (stessa funzionalità eseguita dal tasto Fire e +);
     - Preheat - settaggio di preriscaldamento per il profilo attivo;
     - Edit Profile - entra nel menù del profilo;
     - Smart On/Off
     - Show Info Screen - mostra informazioni;
* **RTC** - impostazione orologio realtime ;
* **Expert** - impostazioni per utenti avanzati:

![](http://i.imgur.com/UZBrHjJ.png) ![](http://i.imgur.com/7fT0pNi.png) ![](http://i.imgur.com/edejq3z.png) ![](http://i.imgur.com/FoH1vaE.png)

* **USB**
     - NoSlp - modalità "dormiente" non contemplata quando connesso sulla porta USB;
     - Charge - il dispositivo carica le batterie quando connesso alla porta USB;
* **BVO** - offset voltaggi batterie;
* **BATT** - profilo di scarica batteria;
* **SHUNT** - Correzione del misuratore di Ohm;
* **ChkTCR** - controllo del materiale TCR, disattivando quest'opzione si possono eliminare errori TCR su bobine pesanti;
* **RCOBC** - Resetta i contatori al cambio batteria, resettando anche le statistiche dello svapo;
* **X32** - Il modulo RTC module usa un oscillatore a 32768 Hz, se presente;
* **LSL** - Light Sleep Mode, per dispositivi senza oscillatore secondario per mantere l'RTC accurato. Potrebbe causare battery draining nella modalità standby, l'utente verrà notificato dell'attività di questa modalità con il simbolo "!" nei pressi della batteria.
* **TEMP** - sensore per la temperatura del circuito, Ext - board temperature sensor, Ext - termistore, Int - MCU


## Info Screen
![](http://i.imgur.com/2QoKfkX.png)

Mostra brevi informazioni hardware e alcune statistiche.

### Ringraziamenti:
     * TBXin - per i prodotti NFE, idee e test
     * Zinger - per le grafiche, idee e test
     * ClockSelect - for great project called myevic

# Disclaimer:
Il firmware è distribuito nella speranza che possa essere utile, ma senza alcuna garanzia. Esso è fornito "così com'è", senza alcun tipo di garanzia, espressa o implicita, comprese, ma non limitatamente alle garanzie implicite di commerciabilità e idoneità per uno scopo particolare. 
I rischi per quanto riguarda la qualità e le prestazioni del firmware sono da ritenersi esclusivamente a carico dell'utente finale.
# Donazioni:
Se ti piace il nostro progetto e vuoi aiutare nel suo sviluppo, è possibile [donare](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=ZLFDYGBRXQJGE) .
