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
