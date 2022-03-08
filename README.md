[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2653146.svg)](https://doi.org/10.5281/zenodo.2653146)

# MaxBotix-Helper
This board connects to a MaxBotix "weather-resistant" series ultrasonic rangefinder to present a friendlier set of output pins with screw terminals for easy hookup.

| **Top** | **Bottom** |
| ------- | ---------- |
| <img src="https://github.com/NorthernWidget-Skunkworks/MaxBotix-Helper/blob/master/doc/OSHParkTop.png" width="280"> | <img src="https://github.com/NorthernWidget-Skunkworks/MaxBotix-Helper/blob/master/doc/OSHParkBottom.png" width="280"> |

(Images rendered by OSHPark)

### Materials for full assembly
* 1 MaxBotix ultrasonic rangefinder (https://www.maxbotix.com/)
* (Optional) 1 MaxBotix "MaxTemp" temperature correction (https://www.maxbotix.com/Ultrasonic_Sensors/MB7955.htm)
* 1 1x6 screw terminal block, 0.1" spacing (https://www.digikey.com/product-detail/en/on-shore-technology-inc/OSTVN06A150/ED10565-ND/1588866)
* 1 1x7 stubby male header (https://www.digikey.com/product-detail/en/samtec-inc/TSW-107-06-T-S/SAM1027-07-ND/1101220)

### Pins
* **GND:** Ground
* **TC:** Temperature correction for optional MaxTemp sensor
* **SIG:** Signal, selectable to *analog* or *serial* (UART) based on solder jumper connection
* **V+:** Input voltage

### Features
* 1 3-pin output for the temperature correction (2x GND + 1x TC)
* 1 3-pin output for the data logger or other microcontroller, etc. interface (GND, V+, SIG)
* Includes the proper number of ground connections to link both the temperature correction and the data logger to the MaxBotix rangefinder (3 instead of 1)
* Selectable output: analog voltage or serial signal

### Instructions
* User solder to select an analog or serial output on bottom side of the board
* Solder the male header terminal onto the top side of the board
* Using the male header terminal block, solder the MaxBotix-Helper to your MaxBotix rangefinder, oriented such such that the black plastic piece in the center lies along the widest point of the threaded circular housing. If you are unsure, match up the white square on our Helper with the square pin on the MaxBotix solder rings. This is the critical piece: otherwise, the new assembly will not fit in a 3/4" pipe, according to the sensor threading!
* Solder the screw terminal block onto the top side of the board (you can also do this earlier, depending on when it is easier for you). This should be in the position that makes it centered within the threaded circular ring.

That's it! At this point, you should be ready connect your data logger / MCU device and the optional MaxTemp sensor. The last steps are just to ruggedize your sensor if you use it outside: we recommend press-fit PVC connections to prevent the wire-to-board connections from shearing off, and to use a solar radiation shield for the temperature compensation sensor.
