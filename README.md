# esphome_qalcosonicnfc
ESPHome component for reading an Axioma Qalcosonic W1 water meter via a PN5180 NFC chip

## Needed components
- ESP32 or ESP8266 (Wemos D1 mini)
- PN5180-NFC module (Can be easily obtained via AliExpress. I paid around 5 USD in August 2025.)
- Some breaboard cables
- (Perfboards)

## Wiring
| ESP32 Pin | PN5180 Pin | ESP8266 Pin (Wemos D1 mini) |
| :---      | :---       | :---                        |
| VIN / 5V  | 5V         | 5V                          |
| 3.3V      | 3.3V       | 3V3                         |
| GND       | GND        | G                           |
| SCLK, 18  | SCLK       | D5                          |
| MISO, 19  | MISO       | D6                          |
| MOSI, 23  | MOSI       | D7                          |
| 14        | NSS        | D1                          |
| 16        | BUSY       | D2                          |
| 17        | RST        | D3                          |

## Special Thanks
Special thanks goes to @ATrappmann for his PN5180-Library (https://github.com/ATrappmann/PN5180-Library).
Without his work, this project would not have been possible.

## Example configuration

See [qalco_conf.yaml](./qalco_conf.yaml)

## Images
<img src="./media/esp32_pn5180_1.jpg" width="200" /> <img src="./media/esp32_pn5180_2.jpg" width="200" /> <img src="./media/esp32_pn5180_3.jpg" width="200" />
