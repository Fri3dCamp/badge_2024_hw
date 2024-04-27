# Badge 2024 hardware
In deze Git repository kan je de ontwerp bestanden en productie data terug vinden van de [Fri3d Camp](https://fri3d.be/) 2024 badge
Revisie 01 is de versie die op kamp zal uitgedeeld worden.

De badge is gebouwd rond de Espressif [ESP32-S3-WROOM-1-N16R8](Datasheets/esp32-s3-wroom-1_wroom-1u_datasheet_en.pdf) module met 16MB flash en 8MB PSRAM. De [ESP32-S3](Datasheets/esp32-s3_datasheet_en.pdf) is een dual-core Xtensa LX7 microcontroller (geklokt aan 240MHz) met Wi-Fi en Bluetooth 5 ondersteuning. Daar deze microcontroller zelf een USB interface heeft is er geen nood meer om een USB serial brug te voorzien zoals op de [badge van 2022]( https://github.com/Fri3dCamp/badge-2020) en de [badge van 2018]( https://github.com/Fri3dCamp/badge). Verder hebben we de badge uitgerust met een [6-assige IMU van Würth Elektronik](Datasheets/Wurth-WSEN-ISDS.pdf), een buzzer, een hoop knopen, een joystick, een microSD kaart lezen en een prachtige [2” IPS LCD met afgeronde hoeken](Datasheets/QT020JA001-A0_SPEC.pdf). Er is wederom een [2de voeding](Datasheets/xc6210.pdf) geplaatst om de Wi-Fi module afzonderlijk van voeding te voorzien, in deze versie hadden we gelukkig genoeg vrije I/O om deze 2de voeding ook aan te kunnen sturen. Om energie te besparen kan je deze dus uitschakelen, enkel de ESP32-S3 zal dan nog stroom krijgen. Om het geheel van stroom te voorzien gebruiken we deze keer een [2000mAh lithium polymeer cel](Datasheets/2000mAh 704060 batterij specific-Tewaycell.pdf) met een ingebouwd protectie circuit. Deze batterijen zijn echter mechanisch niet zo sterk als de 18650 cellen die we in vorige editie gebruikten, daarom zal de badge standaard een cover hebben om deze te beschermen. Om het geheel op te laden via de ingebouwde USB-C poort maken we wederom gebruik van de [TP4056 lineaire lader](Datasheets/TP4056.pdf). Uiteraard is er weer een plek voorzien om de [nieuwe blaster]( https://github.com/Fri3dCamp/blaster_2024) aan te sluiten (ook [die van 2022]( https://github.com/Fri3dCamp/timeblaster-2020) is compatibel met deze badge!). Verder hebben we plek voorzien voor een [SAO header]( https://hackaday.com/2019/03/20/introducing-the-shitty-add-on-v1-69bis-standard/) en is er onderaan een eigen uitbreidingsconnector waar je makkelijk draadje in kan steken om te experimenteren.

![Badge 2024 00 Front](Media/Badge_Front.png)

![Badge 2024 00 Back](Media/Badge_Back.png)

# Badge 2024 hardware (EN)
This repository contains the hardware design and production files for the [Fri3d Camp](https://fri3d.be/en/) 2024 badge.
Revision 01 will be handed out during the event.


