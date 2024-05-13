# I2C Scanner

This Arduino script scans for devices connected via the I2C bus and reports their addresses. It is useful for troubleshooting and setting up a network of I2C devices.

## Features

- **Compatibility:** Works with any Arduino-compatible board.
- **Output:** Lists the addresses of all detected I2C devices.
- **Error Handling:** Reports unknown errors encountered during scanning.

## Requirements

- An Arduino board (e.g., Uno, Mega, Leonardo)
- Arduino IDE for uploading the script to the board
- At least one I2C device connected to your Arduino

## Setup

1. Connect your Arduino board to your computer.
2. Open the Arduino IDE.
3. Connect the I2C devices to the Arduino following standard I2C wiring protocols (SDA to A4, SCL to A5 on an Arduino Uno).
4. Upload this script to your Arduino board.

## Usage

After uploading the script to your Arduino:
1. Open the Serial Monitor from the Arduino IDE.
2. Set the baud rate to `9600`.
3. The scanner will automatically start scanning the I2C bus every 5 seconds.
4. Observe the Serial Monitor output for device addresses or any error messages.

## Example Output

```text
I2C Scanner
Scanning...
I2C device found at address 0xXX  !
...
No I2C devices found
done
