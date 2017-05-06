### *Preliminaire*
# ArcticFox
*[NFE Team](http://nfeteam.org) présente le firmware custom pour les mods Joyetech, Wismec et Eleaf*

```
```

**Utilisez [NFE Toolbox](https://github.com/TBXin/NFirmwareEditor/releases) pour [installer](https://github.com/maelstrom2001/ArcticFox/wiki/How-to-install) le firmware et configurer votre appareil.**

## Liste des appareils supportés:
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
La sécurité d'utilisation de notre firmware est l'un de nos buts premier. Nous conservons toutes les sécurités d'usine car le fabricant ne les a pas conçu "juste pour rire".
Quelles sont les limitations?
* Résistance minimale (Pour les appareils compatibles)
  * 0.05 Ohm pour le mode de controle de température
  * 0.1 Ohm pour le mode Vari-Watt
* Puissance en watt (dépendant de l'appareil)
* Courant maximum de charge (dépendant de l'appareil)
* Courant maximum de sortie (dépendant de l'appareil)
* Plage de sortie en volt (dépendant de l'appareil)

"Dépendant de l'appareil" signifie que chaque appareil possède ses propres valeurs qui sont choisies par le fabricant. Vous pouvez trouver ces valeurs sur la page produit du site internet de votre fabricant.

**Toutes demandes pour changer ces valeurs seront rejetés car nous ne voulons pas vous blesser ou endommager votre appareil.**

## Profils
La principale différence est une interface basé sur les profils, en d'autre terme: le style DNA; ainsi qu'une personnalisation plus poussé que le firmware original Joyetech.
Les profils sont un ensemble de paramètre dépendant d'un atomizer, comme le type de coil, sa résistance, la puissance ou la température nécessaire.
L'utilisateur dispose de 8 profils qui peuvent être édité à l'aide de NFE Toolbox et qui sont assignables par atomizer.

![](http://i.imgur.com/GF9vAbN.gif) ![](http://i.imgur.com/n7IAwpv.gif)

Les profils peuvent être chargés automatiquement selon la valeur de résistance du coil enregistré ou alors de façon manuelle. Pour utiliser le mode de selection automatique, il suffit d'activer le mode "Smart", installer un atomizer et l'assigner au profil souhaité.

![](http://i.imgur.com/J8TXMpU.png) ![](http://i.imgur.com/PvMv2at.png)

Lorsque vous réinstallez l'atomizer plus tard, le profil correspondant s'activera automatiquement.
Si la résistance de l'atomizer installé n'est pas reconnu dans les profils, vous serez amené à choisir un nouveau profil ou à réassigner un existant.

Lorsque vous changez de profil manuellement et que la valeur de résistance sauvegardé est différente, vous devrez confirmer la réassignation ou l'abandon du remplacement de profil.

![](http://i.imgur.com/2u0Jgwb.png) ![](http://i.imgur.com/prrhsrr.png)


## Ecran principal

![](http://i.imgur.com/ARKJkRS.gif)

L'édition de l'écran principal est différente du firmware original Joyetech. Pour éditer les éléments de l'écran principal, activez l'action "Edit Main" (4 appuis sur le bouton Fire par défaut). Un seul appui sur Fire sélectionnera le prochain élément éditable. Modifiez la valeur en utilisant les boutons de régulation. Pour quitter le mode d'édition, maintenez le bouton Fire environ 1 seconde.

## Menu principal

Maintenez les boutons Fire et Plus (par défaut) pendant 1 seconde pour accéder au menu

![](http://i.imgur.com/feb0TFy.png)

### Menu Profil

![](http://i.imgur.com/k5lilx4.png) ![](http://i.imgur.com/5ZPdPL1.png) ![](http://i.imgur.com/eVM4jxZ.png) ![](http://i.imgur.com/6874bnH.png)

* **Wire** - Type de fil, Mode température ou non (VW), peuvent être mis sur standard ou personnalisé TFR;
* **Coil** - Valeur sauvegardé de la résistance du coil;
* **TCR** - valeur pouvant être édité quand l'option Joyetech TC avec TCR personnalisé est activée;
* **T. Dom** - Mode de régulation à température dominante;
* **Preheat** - Contrôle de puissance, utilise la préchauffe ou une courbe de puissance;
* **PI-Reg** - Régulateur PI en mode TC, améliore la puissance et la stabilité en température:
     - PI-Reg On/Off - Selectionne le mode Joyetech par défaut ou personnalisé
     - Range - 0..100% - Étendu de température quand la régulation PI devient active. 0 signifie que la régulation est toujours active et contrôle la distribution de puissance dès le début, 20% par exemple - La régulation PI s'active quand la température du coil atteint 20% de la température du profil;
     - P - Constante proportionnelle, plus la valeur est importante, plus rapide sera le changement de puissance;
     - I - Constante intégrale, plus la valeur est importante, plus la puissance sélectionné sera appliqué de façon lisse.

### Screen Menu

![](http://i.imgur.com/ANnqWiG.png) ![](http://i.imgur.com/Z5ygFZR.png) ![](http://i.imgur.com/IKs6AeP.png) ![](http://i.imgur.com/u2wvplG.png) ![](http://i.imgur.com/f4pXIRN.png) ![](http://i.imgur.com/ozrsc7q.png)

* **Wake <>** - Réactive l'appareil en pressant les boutons de régulations;
* **Logo** - Affiche le logo sur l'écran princiapl;
* **Clock**
     - **Type** - Analogique ou digitale;
     - **On Main** - Affiche l'horloge sur l'écran principal;
     - **Saver** - Affiche l'horloge en mode veille;
* **Timeouts**
     - **Dim** - Temps d'inactivé avant que l'écran ne s'éteigne;
     - **Dim** :lock: - Temps d'inactivité avant que l'écran ne s'éteigne en mode bloqué;
     - **Logo** - Temps d'inactivité avant que le logo n'apparaisse;
     - **Clock** - Temps d'inactivité avant que l'heure n'apparaisse;
* **Charge**
     - **Type** - Type d'écran pendant la charge, standard ou avec des informations complémentaires;
     - **Add.** - Élément additionnels, horloge ou logo;
* **Stealth** - Paramètres pour l'écran en mode Stealth:
     - **Charge** - L'écran de chargement sera affiché en mode Stealth;
     - **Saver** - L'écran de veille sera affiché en mode Stealth;
     - **ClkOnF** - Quand l'option "Horloge sur l'écran principal" est active, l'horloge sera affiché immédiatement après un appui sur le bouton Fire;
* **Contrast** - Ajuste la luminosité de l'écran;
* **Skin** - Change le style de l'écran principal.

### Menu paramètre

![](http://i.imgur.com/iWCQH2q.png) ![](http://i.imgur.com/mQYC7Vi.png) ![](http://i.imgur.com/24Oqlur.png) ![](http://i.imgur.com/mS1hiZY.png)

* **1 Watt** - Incrémente/Décrémente la puissance par pas de 1.0 Watt;
* **Clicks** - Actions assignés pour
     * **2/3/4 appuis sur le bouton Fire**:
          - None - Rien;
          - Edit Main - Mode édition Joyetech par défaut en 3 clics;
          - Main Menu - Entrer dans le menu principal, identique à Fire et +;
          - Preheat - Paramètre de préchauffe pour le profil actif;
          - Profiles - Sélecteur de profil;
          - Edit Profile - Entre dans le menu d'édition de profil;
          - T. Dom - Mode température dominante On/Off;
          - Clock - Affiche/Cache l'horloge sur l'écran principal;
          - Info - Affiche la page d'information;
          - Reset Cnt. - Affiche les stats de vape et l'option pour réinitialiser les compteurs;
          - Power Bank - Active le mode de recharge Power Bank;
          - Coil Lock - Blocage de la valeur de résistance du coil On/Off (pour les modes TC);
          - Key Lock - Blocage des touches de régulations On/Off;
          - Stealth - Mode Stealth On/Off;
          - Smart On/Off - Mode Smart On/Off;
          - LSL - Mode sommeil léger On/Off;
          - Device Lock - Mode bloqué On/Off (bloque tous les boutons mais laisse l'appareil allumé);
          - On/Off - Allume/Éteint On/Off;
     * **5 appuis sur le bouton Fire**:
          - Device Lock - Mode bloqué On/Off (bloque tous les boutons mais laisse l'appareil allumé);
          - On/Off - Allume/Éteint On/Off.
* **Smart** - Changement automatique de profil:
     - Off/On/Lazy - Fonctionnement du mode Smart: "Lazy" signifie que le profil peux être changé automatiquement uniquement lors d'un changement d'atomizer lorsque l'appareil est actif;
     - Range - Tolérance de résistance;
* **Clock** - Horloge temps-réel;
     - Date/Time - Ajuster la date et l'heure;
     - Adjust Time - Ajuster l'heure par palier d'une seconde pour les psychorigides;
     - LIRC Speed - Ajuste la vitesse de l'oscillateur interne imprécis pour les appareils sans crystal externe 32768 Hz;
* **Expert** - Paramètres pour les utilisateurs avancées:

![](http://i.imgur.com/TewKhaq.png) ![](http://i.imgur.com/t24VXIO.png) ![](http://i.imgur.com/7feR2HK.png) ![](http://i.imgur.com/KqArvHQ.png)

* **USB**
     - NoSlp - Ne pas entrer en mode de sommeil profond quand l'appareil est connecté en USB - peux provoquer une décharge sur les multi-cells après que la charge soit terminée;
     - Charge - L'appareil se recharge quand il est connecté en USB - seulement pour les appareils multi-cells;
* **BVO** - Décalage de voltage de batterie;
* **BATT** - Profil de décharge de batterie;
* **SHUNT** - Correction du Ohmmètre;
* **ChkTCR** - Vérifie le type de fil du coil en TCR, désactiver cette option peux éliminer les erreurs en TCR avec les gros coils;
* **RCOBC** - Remise à zéro des compteurs et des statistiques de vape lors du changement de batterie;
* **RTC** - Mode de l'horloge temps-réel:
     - LXT - Support hardware complet;
     - LIRC - Second oscillateur imprécis;
     - LSL - Mode logiciel. Il consomme un peu plus d'énergie en mode veille mais procure des résultats plus précis sur les appareils sans horloge temps-réel matériel;  
     ***Note***: Après un changement du mode d'horloge, débranchez le câble USB et redémarrez votre appareil en retirant les batteries pendant 30 secondes.
* **TEMP** - Type de capteur de température de la carte, Ext - thermistance, Int - MCU;
* **D. Sleep** - Mode de veille profonde (entre après 3 minutes d'inactivité):
     - Std - Veille profonde standard;
     - Power / Lock - Éteint/Bloque l'appareil avant d'aller en veille profonde.

### Power Bank

![](http://i.imgur.com/IxyXhex.png) ![](http://i.imgur.com/pnfnHQ0.gif) ![](http://i.imgur.com/D8dLPZJ.gif)

Support des adaptateurs Avatar RC et similaire. Donne un voltage de 5 volts et un courant pouvant aller jusqu'a 2.1 ampères. Pour démarrer la charge, mettez l'adaptateur sur l'appateil, connectez un appareil et pressez le bouton Fire. Le mode Power Bank à un mode de coupure quand le courant tiré est inférieur à 50 mA (indiqué par le clignotement de l'étiquette "On"). Pour arrêter la charge, appuyez sur le bouton Fire.
Pour quitter le mode Power Bank, appuyez et maintenez le bouton Fire ou les boutons de régulations simultanément.


### Ecran d'information

![](http://i.imgur.com/bsXlfpV.png) ![](http://i.imgur.com/5FG1OD6.gif)

Affiche de brèves informations et quelques statistiques.

### Remerciements à:

* **TBXin** - pour la partie NFE et l'aide au développement
* **Zinger** - pour les graphiques, idées et tests
* **ArionWT** - pour les graphiques, idées et tests
* **ClockSelect** - pour le super projet nommé myevic

# Avertissement:

Le firmware est distribué dans l'espoir qu'il sera utile, mais sans aucune garantie. Il est fourni "tel quel" sans aucune garantie d'aucune sorte, autant explicite qu'implicite, incluant, mais non limité, les garanties implicites de qualité marchande et de conditionnement physique à des fins particulières. Le risque entier tant en qualité qu'en performance n'est imputable qu'a vous.

# Donations:
Si vous aimez notre projet et que vous souhaitez aider à son développement, vous pouvez [faire un don](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=ZLFDYGBRXQJGE) du montant que vous estimez acceptable.
