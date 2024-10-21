# CAN Based NTC Daughter Board
#### Client Name: Dewald Le Grange

## Project Requirements - v1
The board aims to act as a secondary board in a CAN network providing Temperature related info the main master in the network. The core requirements of the design are highlighted below:

### Core Features
- Suitable ESP32 (pre-certified) with sufficient Non-volatile memory for the application (This means a module with decent Flash should be picked).
- Isolated DC/DC for power with support of voltage range from 10V - 30V (EV running on 12V and out BESS systems on 24V). Necessary polarity and input range protection should be added as well.
- CAN Transceiver. It is advised to use a module variant with built-in CAN Controller to avoid extra circuitry on board.
- The 8x NTC will connect to ESP32 via an external connector. The ESP32 ADC should be utilized to read value, or an additional ADC should be introduced on board in order to not compromise accuracy. Necessary analog filters and protection should be added to have precise and accurate analog readings.
- The board will feature 3 x connectors as below:
    - 16 Pin Connector for NTC termination: PN: 10142344-116KLF
    - 5 Pin Connector IN: 10142344-104KLF
        - Power
        - GND
        - CANH
        - CANL
    - 5 Pin Connector OUT: 10142344-104KLF
        - Power
        - GND
        - CANH
        - CANL

### Specifications
- NTC +-1% Accuracy
- The temperature range will be -20 to 60°C,

### Board Dimensions
![image](https://github.com/user-attachments/assets/9ff1a8d9-cd38-4594-8c93-7d55fc0aac09)



