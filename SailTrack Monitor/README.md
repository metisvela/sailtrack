# SailTrack Monitor
The SailTrack Monitor module is an output-only module, that means that it is a module that doesn't publish messages on the network, but it only recceives them instead. In fact, it does not contain any sensor, as its main purpose is to show some key metrics to the boat crew. The module is composed by an ESP32 microcontroller (that connects to the SailTrack Network) and an e-paper display, to display the metrics in a clear way, even under conditions with a lot of sunlight. In fact, the readability of e-paper displays is really high, with the downside that they have really high refresh time.

The module performs the following tasks:

* It gets the metric from the network and displays them in the e-paper monitor.

The module is mounted in a closed waterproof enclosure and it is placed under the boom, in a position such that it can be easily seen by the crew.

![monitor-image](Assets/Monitor%20Image.jpg)

## Resources
* [Module Repository](https://github.com/metis-vela-unipd/sailtrack-monitor)
