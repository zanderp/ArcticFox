# ArcticFox
*Il [team NFE](http://nfeteam.org) presenta un custom firmware per le battery mod Joyetech, Wismec ed Eleaf*

![](http://i.imgur.com/PqSrmLb.png) ![](http://i.imgur.com/C8Lu9SG.png) ![](http://i.imgur.com/aBhNKxV.png) ![](http://i.imgur.com/rk6gZo8.png) ![](http://i.imgur.com/5mU3FAB.png) ![](http://i.imgur.com/wl8wR8d.png) ![](http://i.imgur.com/s3yNIEf.png)

**Utilizza l'[NFE Toolbox](https://github.com/TBXin/NFirmwareEditor/releases) per [installare](https://github.com/maelstrom2001/ArcticFox/wiki/How-to-install) il firmware e per configurare il tuo dispositivo.**

## Lista delle battery mod supportate:
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
* VS Switchbox
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
* iStick QC 200W

 ## Limitazioni
L'utilizzo in tutta sicurezza del nostro software è uno dei nostri obiettivi principali. 
E' per questo motivo che conserviamo tutte le restrizioni imposte dal produttore.
Semplicemente, non sono state messe lì per caso e per questo riteniamo sia importante tenerne conto.
Quali sono queste restrizioni?
 * Valore minimo delle resistenze (Per tutti i dispositivi supportati)
   * 0.05 Ohm per le resistenze usate in Temperature Control
   * 0.1 Ohm per le resistenze usate in Vari-Watt
  * Massimo valore di corrente in carica (Dipende dal dispositivo)
  * Output massimo di corrente (Dipende dal dispositivo)
  * Range del voltaggio in uscita(Dipende dal dispositivo)

La dicitura "Dipende dal dispositivo" significa, per l'appunto, che ogni dispositivo ha i suoi valori limite, scelti dal produttore.
Questi valori possono essere trovati sul sito del produttore della vostra box.
 
 **Tutte le richieste riguardanti modifiche di questi valori saranno categoricamente rifiutate. Non vogliamo che voi utenti possiate arrecare danno alle vostre box o alla vostra persona.**
 
## Profili
La differenza principale è l'interfaccia utente, simile a quella DNA, pienamente modificabile rispetto al firmware originale Joyetech.
I profili sono composti da set di parametri utilizzati dall'atomizzatore come il materiale delle coil, le resistenze, potenza erogata e valori relativi alle temperature.
L'utente ha a disposizione 8 profili personalizzabili attraverso la NFE toolbox, che può assegnare liberamente al suo atomizzatore preferito.

![](http://i.imgur.com/GF9vAbN.gif) ![](http://i.imgur.com/n7IAwpv.gif)

I profili possono essere cambiati automaticamente sulla base dei dati raccolti dal firmware oppure in modalità manuale.
Per far si che il firmware utilizzi questa funzione è necessario abilitare la "Smart" mode, installare l'atomizzatore ed assegnarlo al profilo desiderato.

![](http://i.imgur.com/J8TXMpU.png) ![](http://i.imgur.com/PvMv2at.png)

Quando reinstallerai l'atomizzatore più tardi, il profilo precedentemente assegnato verrà attivato automaticamente.
Se la resistenza dell'atomizzatore installato non viene trovato nei profili, verrà chiesto all'utente di assegnarne uno nuovo o di riassegnare un profilo esistente.
Quando l'utente cambia manualmente il profilo e la resistenza non combacia con i dati inclusi nello stesso, verrà chiesto se mantenere la precedente configurazione o aggiornarla.

![](http://i.imgur.com/2u0Jgwb.png) ![](http://i.imgur.com/prrhsrr.png)


## Main Screen

![](http://i.imgur.com/ARKJkRS.gif)

La modifica dello schermo principale si differenzia dai firmware originali di Joyetech. Per modificare gli elementi nella schermata principale, utilizza l'azione "Edit Menu" (4 pulsanti Fire pulsante per impostazione predefinita). La pressione singola del pulsante Fire commuterà l'azione sull'elemento successivo disponibile da modificare. Si potrà modificare l'elemento selezionato premendo i pulsanti regolatori. Per uscire dalla modalità di modifica basta tenere premuto il pulsante di accensione per circa 1 sec.

## Main Menu

Tenere premuti i pulsanti Fire e Plus (per impostazione predefinita) per 1 secondo per entrare nel Main Menu.

![](http://i.imgur.com/feb0TFy.png) ![](http://i.imgur.com/be2BWSt.png)

### Profile Menu

![](http://i.imgur.com/k5lilx4.png) ![](http://i.imgur.com/5ZPdPL1.png) ![](http://i.imgur.com/eVM4jxZ.png) ![](http://i.imgur.com/6874bnH.png)
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

### Screen Menu

![](http://i.imgur.com/ANnqWiG.png) ![](http://i.imgur.com/Z5ygFZR.png) ![](http://i.imgur.com/IKs6AeP.png) ![](http://i.imgur.com/u2wvplG.png) ![](http://i.imgur.com/f4pXIRN.png) ![](http://i.imgur.com/ozrsc7q.png)
* **Dim** - timeout del display;
* **Wake <>** - risveglia la mod premendo i pulsanti regolatori;
* **Charge** - mostra informazioni accessorie sulla schermata di caricamento, voltaggi della batteria e temperatra del circuito;
* **Logo** - mostra il logo sulla schermata principale;
* **Clock**
     - **Type** - analogico o digitale;
     - **On Main** - mostra l'orologio sulla schermata principale;
     - **Saver** - mostra l'orologio nella modalità standby;
* **Timeouts**
     - **Dim** ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - modifica i secondi che impiegherà lo schermo prima di bloccarsi;
     - **Logo** - tempo d'inattività prima che il logo venga mostrato;
     - **Clock** - tempo d'inattività prima che l'orologio venga mostrato;
* **Charge**
     - **Type** - permette di selezionare la tipologia di schermata per la ricarica tra standard o con informazioni aggiuntive;
     - **Add.** - opzioni extra, orologio o logo;
* **Stealth** - impostazioni dello schermo in modalità stealth:
     - **Charge** - la schermata di ricarica viene mostrata nella modalità Stealth;
     - **Saver** - lo screen saver viene mostrato nella modalità stealth;
     - **ClkOnF** - quando l'opzione "Clock On Main Screen" è attivata, l'orologio sarà mostrato immediatamente alla singola pressione del tasto Fire;
* **Contrast** - modifica la luminosità dello schermo;
* **Skin** - cambia la skin .

### Settings Menu

![](http://i.imgur.com/iWCQH2q.png) ![](http://i.imgur.com/mQYC7Vi.png) ![](http://i.imgur.com/24Oqlur.png) ![](http://i.imgur.com/mS1hiZY.png)

* **1 Watt** - incrementa/decrementa la potenza di 1,0 Watt;
     - On/Off;
     - tolleranza resistenza;
     - mostra il Profile Menu dopo averne assegnato uno nuovo;
* **Clicks** - actions assigned on
     * **2/3/4 Fire button clicks**:
          - None;
          - Edit Main - Azione di default eseguita dai 3 click sul firmware Joytech;
          - Main Menu - entra nel menù principale, stessa funzionalità della combinazione Fire e +;
          - Preheat - impostzioni di preriscaldamento per il profilo attivo;
          - Profiles - selettore profili;
          - Edit Profile - entra nel Menù dei Profili;
          - T. Dom - temperature-dominant on/off;
          - Clock - mostra/nasconde l'orologio sulla schermata principale;
          - Info - mostra la schermata delle informazioni;
          - Reset Cnt. - mostra le statistiche di svapo con l'opportunità di resettarle;
          - ![](https://cdn4.iconfinder.com/data/icons/font-awesome-2/2048/f011-16.png) Bank - attiva la modalità power-bank;
          - Coil ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - attiva/disattiva il blocco resistenza (modalità TC);
          - Key ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - attiva/disattiva blocco tasti;
          - Stealth - attiva/disattiva la modalità Stealth;
          - Smart On/Off - attiva/disattiva la modalità Smart;
          - LSL - attiva/disattiva la modalità "light sleep";
          - Device ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - attiva/disattiva la modalità "blocco dispositivo" (tutti i pulsanti vengono bloccati ma la mod resta accesa);
          - On/Off - attiva/disattiva la box;
     * **5 Fire button clicks**:
          - On/Off - attiva/disattiva la box;
          - Device ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - attiva/disattiva la modalità "blocco dispositivo" (tutti i pulsanti vengono bloccati ma la mod resta accesa);
* **Smart** - cambio automatico delle impostazioni dei profili:
     - Off/On/Lazy - Smart Mode behavior setting, Lazy means that profile can be switched automatically only on atomizer change while the box is in active state;
     - Range - resistance tolerance;
* **Clock** - realtime clock setup;
     - Date/Time - imposta data e ora;
     - Adjust Time - impostazione precisa dell'ora tramite la gestione dei secondi;
     - LIRC Speed - impostazione per correggere la velocità interna dell'oscillatore impreciso della box (da utilizzare sulle box che non hanno il cristallo esterno a 32768Hz;
* **Expert** - impostazioni per utenti avanzati:

![](http://i.imgur.com/TewKhaq.png) ![](http://i.imgur.com/t24VXIO.png) ![](http://i.imgur.com/7feR2HK.png) ![](http://i.imgur.com/pp3TTaR.png)
* **USB**
     - NoSlp - modalità "dormiente" non contemplata quandola box è connessa tramite USB;
     - Charge - il dispositivo carica le batterie quando la box è connessa tramite USB;
* **BVO** - offset voltaggi batterie;
* **BATT** - profilo di scarica batteria;
* **SHUNT** - Correzione del misuratore di Ohm;
* **ChkTCR** - controllo del materiale TCR, disattivando quest'opzione si possono eliminare errori TCR su bobine pesanti;
* **RCOBC** - Resetta i contatori al cambio batteria, resettando anche le statistiche dello svapo;
* **RTC** - Modalità Realtime Clock :
     - LXT - per box con pieno supporto hardware;
     - LIRC - con oscillatore secondario non accurato;
     - LSL - modalità software. Consuma un po' più di energia in standby mode, ma ha risultati più accurati su box che non hanno un'implementazione RTC;  
     ***Nota***: dopo la commutazione nella RTC mode, disconnetti al box dalla porta USB e riavviala togliendo le batterie per circa 30 secondi.
* **TEMP** - temperatura rilevata dal sensore, Ext - thermistor, Int - MCU;
* **D. Sleep** - modalità deep sleep (dopo 3 minuti di inattività):
     - Std - standard deep sleep;
     - ![](https://cdn4.iconfinder.com/data/icons/font-awesome-2/2048/f011-16.png) - la box viene spenta prima di entrare in modalità deep sleep;
     - ![](https://cdn2.iconfinder.com/data/icons/font-awesome/1792/lock-16.png) - la box viene bloccata prima di entrare in deep sleep.
### Power Bank

![](http://i.imgur.com/IxyXhex.png) ![](http://i.imgur.com/pnfnHQ0.gif) ![](http://i.imgur.com/D8dLPZJ.gif)

Introdotto il supporto per l'adattatore Avatar RC e similari. Questo permette alla box di erogare 5 volts e corrente fino alle 2.1 amps. Per iniziare la ricarica, inserisci l'adattatore RC sulla box, connetti il dispositivo e premi il pulsante Fire. La modalità Power Bank ha una funziona di auto spegnimento che si innesca quando il drenaggio della corrente non supera le 50mA (indicato dalla schermata lampeggiante "On"). Per fermare la ricarica basta premere il pulsante Fire. Per uscire dalla modalità Power Bank è necessario tenere premuto il tasto Fire, oppure i pulsanti regolatori (+,-) simultaneamente.


### Info Screen
![](http://i.imgur.com/bsXlfpV.png) ![](http://i.imgur.com/5FG1OD6.gif)

Mostra brevi informazioni hardware e alcune statistiche.

### Ringraziamenti:
* **TBXin** - per i prodotti NFE, idee e test
* **Zinger** - per le grafiche, idee e test
* **ClockSelect** - for great project called myevic
* **ArionWT** - for graphics, ideas and tests

# Disclaimer:
Il firmware è distribuito nella speranza che possa essere utile, ma senza alcuna garanzia. Esso è fornito "così com'è", senza alcun tipo di garanzia, espressa o implicita, comprese, ma non limitatamente alle garanzie implicite di commerciabilità e idoneità per uno scopo particolare. 
I rischi per quanto riguarda la qualità e le prestazioni del firmware sono da ritenersi esclusivamente a carico dell'utente finale.
# Donazioni:
Se ti piace il nostro progetto e vuoi aiutare nel suo sviluppo, è possibile [donare](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=ZLFDYGBRXQJGE) .
