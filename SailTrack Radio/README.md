# SailTrack Radio
The SailTrack Radio module is composed by all the sensors and components that use radio signals, that are the GPS receiver and the [LoRa](https://lora-alliance.org) transceiver. The module is based on a [ESP32](https://www.espressif.com/en/products/socs/esp32) microcontroller, that has WiFi capabilities, needed to connect to the SailTrack Network and to exchange messages to the other modules.

The module performs the following tasks:

* It gets the positioning data from the GPS module mounted on-board.
* It transmits data to ground using LoRa. The metrics that are sent to the ground station can arrive from other modules as well, since every module is connected to the network and can send and receive messages.

The module is mounted inside a waterproof enclosure and it is mounted on the boat spreaders.

![radio-image](Assets/Radio%20Image.jpg)

## Resources
* [Module Repository](https://github.com/metis-vela-unipd/sailtrack-radio)
