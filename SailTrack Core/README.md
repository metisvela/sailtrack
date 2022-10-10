# SailTrack Core
The SailTrack Core module is, as the name says, the main component of the system. It's in fact the only essential component for the SailTrack System. The module is based on a Raspberry Pi SBC, that runs the SailTrack Core OS, a modified version of the [DietPi](https://dietpi.com) OS, which is an ultra-lightweigth, highly-optimized version of the official Raspberry Operating System, namely, [Raspberry Pi OS](https://www.raspberrypi.com/software/).

SailTrack Core is an essential component for the system because it performs the following tasks:
 * It creates the SailTrack-CoreNet, the WiFi network needed by all the modules to communicate.
 * It acts as the [MQTT](https://mqtt.org) Broker, managing the exchange of MQTT messages between modules.
 * It runs the [InfluxDB](https://www.influxdata.com) database, gathering all the measurements coming from the sensors.
 * It runs the [Grafana](https://grafana.com) server, for the visualization of real-time and logged metrics.
 * It processes the readings coming from the sensors by filtering and combining them to obtain derived metrics.
 
 The module is protected by a custom, 3D-printed, waterproof enclosure, and it is mounted inside the boat.

![core-image](Assets/Core%20Image.jpg)

## Resources
* [Module Repository](https://github.com/metis-vela-unipd/sailtrack-core)
