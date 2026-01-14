# yoRadio PCF8574 4x4 Keyboard suport

This mod enables the use of 16 buttons to handle favorite stations in yoRadio using a PCF8574 expander. The favorite stations are stored in the ESP32 flash memory. A short button press retrieves the station (if already stored), while a long press (>1 sec) saves the current station to the slot assigned to that button.
<br><br>
The required connections are shown in the file "PCF8574 4x4 Keyboard.jpg".
<br><br>
IMPORTANT:
<br>- If the project uses an external RTC, the I2C's SDA and SCL pins for both the expander and the RTC can be the same (recommended).
<br>- If an I2C display is used in addition to the RTC, then the SDA and SCL pins for the expander must be the same as those used for the RTC!
<br><br>
**Installation**:
<br>1. In Arduino IDE/Pioarduino add add I2CKeyPad library by RobTillaart (https://github.com/RobTillaart/I2CKeyPad).
<br>2. Replace the "player.cpp" file in the "yoradio-main\yoRadio\src\core" directory with the provided one, or manually add the three required sections to the appropriate parts of your "player.cpp" file. Each section to be added is delimited by lines: /**************** EXTENDER ****************/ in the provided "player.cpp" file.
<br>3. In the above mentioned file "player.cpp" set the expander parameters according to your configuration (section: EXPANDER CONFIGURATION)
<br>4. Build & upload
<br><br>Enjoy!
<br>
************************************************************************************************
Ten mod umożliwia wykorzystanie 16 przycisków do obsługi ulubionych stacji w yoRadio za pomocą ekspandera PCF8574. Ulubione stacje są przechowywane w pamięci flash procesora ESP32. Krótkie naciśnięcie przycisku wywołuje stację (jeśli została wcześniej zapisana), natomiast długie naciśnięcie (>1 sek.) zapisuje aktualną stację w slocie przypisanym do danego przycisku.
<br><br>
Wymagane połączenia zostały przedstawione w pliku "PCF8574 4x4 Keyboard.jpg".
<br><br>
WAŻNE:
<br>- Jeżeli projekt wykorzystuje zewnętrzny RTC, piny I2C SDA i SCL ekspandera oraz RTC mogą być takie same (zalecane).
<br>- Jeżeli oprócz RTC wykorzystywany jest wyświetlacz I2C, wtedy dla ekspandera należy wybrać piny SDA i SCL takie jak dla RTC!
<br><br>
**Instalacja**:
<br>1. W Arduino IDE/Pioarduino dodaj bibliotekę I2CKeyPad autorstwa RobTillaart (https://github.com/RobTillaart/I2CKeyPad).
<br>2. Zastąp plik "player.cpp" w katalogu yoradio-main\yoRadio\src\core plikiem z tego repozytorium, lub ręcznie dodaj trzy wymagane sekcje w odpowiednich miejscach pliku "player.cpp". Każda z ww. sekcji jest ograniczona liniami: /**************** EXTENDER ****************/ w dostarczonym pliku "player.cpp".
<br>3. W wyżej wymienionym pliku „player.cpp” ustaw parametry ekspandera zgodnie ze swoją konfiguracją (sekcja: EXPANDER CONFIGURATION).
<br>4. Skompiluj i wgraj (Build & upload)
<br><br>Miłego korzystania!
