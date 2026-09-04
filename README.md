# LED-Matrix-Emoji-Display-System-with-Button-Control

An Arduino project that cycles through seven custom 8×8 emoji designs on a MAX7219 LED matrix when a push-button is pressed.

## Features

- Seven built-in bitmap designs: greeting, faces, apple, and heart
- One-button emoji cycling
- Internal pull-up input wiring
- MAX7219 matrix control through the LedControl library

## Hardware

- Arduino Uno or compatible board
- MAX7219 8×8 LED matrix
- Momentary push-button

## Wiring

| Function | Arduino pin |
| --- | --- |
| Matrix DIN | 12 |
| Matrix CS | 11 |
| Matrix CLK | 13 |
| Button | 5 |

The button uses `INPUT_PULLUP`; wire it between pin 5 and GND.

## Setup

1. Install the **LedControl** library.
2. Open `Source Code` (rename it to `EmojiDisplay.ino` if needed).
3. Connect the matrix and button, then upload.

## Project files

- `Source Code` — Arduino sketch
- `Circuit_image. .png` — wiring reference

## Improvement ideas

- Implement edge-based debouncing rather than a fixed delay.
- Add brightness control with a potentiometer.
- Store additional animations in program memory to conserve SRAM.

## License

No license has been specified. Add one before reusing or distributing this work.