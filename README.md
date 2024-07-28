# GarageDoorMonitor
This project is designed to monitor the state of a garage door using BLE (Bluetooth Low Energy) and Wi-Fi. It scans for BLE signals from a specific sensor and determines whether the garage door is open or closed based on the X-axis values provided by the sensor. ( MINEW E9 sensor)  When the state of the garage door changes, it sends a notification via Telegram.
## Features
- Connects to a specified Wi-Fi network
- Scans for BLE signals from a sensor with a specific MAC address
- Determines the state of the garage door (open or closed) based on X-axis values
- Sends notifications to a Telegram bot when the state of the door changes

## Requirements
- ESP32 development board
- BLE sensor with specified MAC address
- Wi-Fi network credentials
- Telegram bot and chat ID

## Setup
1. Configure the Wi-Fi and Telegram credentials in the code.
2. Deploy the code to an ESP32 development board.
3. Ensure the BLE sensor is active and within range.
4. Monitor the state changes via Telegram notifications.

## Usage
This project continuously scans for BLE signals from the specified sensor and evaluates the X-axis data. If the garage door's state changes (open/closed), a message is sent to the configured Telegram chat.

## Notes
- Ensure the debounce delay is appropriately set to avoid multiple notifications for a single state change.
- The project uses the NimBLE library for efficient BLE scanning.

## License
This project is licensed under the MIT License.
