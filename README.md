The firmware location is: SwitchBlade-X -> Firmware -> SwitchBlade_
# HackPad SwitchBlade-X

## Hardware Overview
- MCU: RP2040
- Matrix: 2x4 (8 Keys)
- Encoder: EC11 Rotary Encoder
- Display: 0.91" SSD1306 I2C OLED
- RGB: 9x SK6812 MINI-E Addressable LEDs

## Firmware Framework
Designed using QMK firmware architecture for:
- Layered key mapping
- Matrix scanning
- Encoder interrupt handling
- I2C OLED communication
- WS2812/SK6812 LED control

## Feature Implementation

### Matrix Scanning
2 row pins, 4 column pins, COL2ROW diode configuration.

### Encoder
Clockwise → Goes up in the keybind layer 
Counter-clockwise → Goes back in the keybind layer

### OLED
Displays:
- Animations
- Which layer you are on while switching

### RGB
Default breathing effect with configurable modes.

## Expansion Ready
Firmware supports:
- Additional layers
- RGB reactive effects
- Encoder layer control
- WPM display
## How to use it?
To use it you have to first customize your firmware according to your needs and then flash the esp and then you can use it easily
I made this project as when i am either coding or doing some robotics stuff i have problem doing some things and to make it easier i have make this hackpad so i can use it for gaming or coding with the encoder chaging the layer of keybinds to use aand the oled and rgb adding the vibe to it
- <img width="852" height="610" alt="Screenshot 2026-03-08 131735" src="https://github.com/user-attachments/assets/6dd65b34-c94a-4fa2-a922-2c503ab8224a" />
<img width="1129" height="718" alt="image" src="https://github.com/user-attachments/assets/07cbf3c3-433c-45fa-b96e-ff4353866491" />
Reference	Qty	Value	DNP	Exclude from BOM	Exclude from Board	Footprint	Datasheet
330ohm1	1	R				Resistor_SMD:R_0201_0603Metric	~
D1,D2,D3,D4,D5,D6,D7,D8	8	1N4148WT				Diode_SMD:D_SOD-523	https://www.diodes.com/assets/Datasheets/ds30396.pdf
D9,D10,D11,D12,D13,D14,D15,D16,D17	9	SK6812MINI-E				footprints:SK6812MINI-E_fixed	https://cdn-shop.adafruit.com/product-files/4960/4960_SK6812MINI-E_REV02_EN.pdf
J1	1	Conn_01x04_Pin				KiCad-SSD1306-0.91-OLED-4pin-128x32:SSD1306-0.91-OLED-4pin-128x32	~
SW1,SW2,SW3,SW4,SW5,SW6,SW7,SW8	8	SW_Push				Button_Switch_Keyboard:SW_Cherry_MX_1.00u_PCB	~
SW9	1	RotaryEncoder_Switch				Rotary_Encoder:RotaryEncoder_Alps_EC11E-Switch_Vertical_H20mm	~
U1	1	MOUDLE-SEEEDUINO-XIAO				footprints:XIAO-Generic-Hybrid-14P-2.54-21X17.8MM	
<img width="1281" height="193" alt="image" src="https://github.com/user-attachments/assets/d56710e1-3da6-47d6-a9b9-21c0b581af13" />

<img width="979" height="500" alt="image" src="https://github.com/user-attachments/assets/9104c812-282c-45e2-a03a-2fc01a09bd57" />
