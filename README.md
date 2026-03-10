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
Clockwise → Volume Up  
Counter-clockwise → Volume Down  

### OLED
Displays:
- Device Name
- Active Layer

### RGB
Default breathing effect with configurable modes.

## Expansion Ready
Firmware supports:
- Additional layers
- RGB reactive effects
- Encoder layer control
- WPM display
- <img width="852" height="610" alt="Screenshot 2026-03-08 131735" src="https://github.com/user-attachments/assets/6dd65b34-c94a-4fa2-a922-2c503ab8224a" />
<img width="1129" height="718" alt="image" src="https://github.com/user-attachments/assets/07cbf3c3-433c-45fa-b96e-ff4353866491" />

