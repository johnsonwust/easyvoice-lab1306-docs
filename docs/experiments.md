# Experiments

Build the offline LED demo first, then test one peripheral at a time. The ideas below describe the intended wiring and behavior. Check the example gallery for your installed AilyBlockly version and adapt the blocks to your firmware.

| Experiment | What to try |
| --- | --- |
| Offline LED control | Load the CI1306 recognition demo and map the two recognized commands to the onboard LED. Check that the serial monitor reports the command. |
| OLED status panel | Use the I²C OLED to show a short message when a command is recognized. Try displaying sensor values next. |
| Real-time clock | Read the PCF85063A over I²C. Add a clock display or timestamp to a sensor reading. A compatible backup battery lets the RTC keep time when the main supply is off. |
| microSD logger | Write dated temperature readings or recognition events to a file over SPI, then reopen the file to check the results. |
| Three-button input | Log the three ADC ranges and map them to menu actions. Start with one button at a time. |
| Ambient light | Compare light readings under a desk lamp and in shade. Use a measured threshold to switch an indicator. The reading is relative to the setup. |
| DHT11 sensing | Read temperature and relative humidity, then use the OLED to display them on demand. |
| PIR motion | Allow the sensor to stabilize after power-on. Use a digital motion event to trigger a light or greeting. |
| WS2812 lighting | Use separate commands to change the color or pattern of the six addressable RGB LEDs. |
| Infrared remote | Capture a button press from a compatible 38 kHz remote. Try transmitting a code to a compatible receiver. Decode and replay depend on the target protocol. |
| DC relay control | Use an appropriate low-voltage DC test load and switch it with a voice command. Start with the output off. |
| ESP32-C3 link | Exchange short messages over 3.3 V UART. Try forwarding a sensor value to a local network application with suitable ESP32-C3 firmware. |
| Motor and servo | Use external DC power. Send a command over I²C to drive a small motor or move a servo within a safe travel range. Test each channel before combining loads. |

See the [hardware guide](hardware.md) for the pins, supply options, and load limits. The [original project notes](https://arduino.me/a/3375) identify the example gallery and the hardware used for each experiment.

[Quick start](quick-start.md) · [Back to README](../README.md)
