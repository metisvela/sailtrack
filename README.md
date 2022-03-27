<p align="center">
  <img src="Graphics/SailTrack Logo.png" width="180">
</p>


<p align="center"><b>Sailing Performance Tracker built by the Métis Vela Unipd team</b></p>

## Introduction
SailTrack is a performance tracker for sailing boats.
This system is built by the Métis Vela Unipd team, a student project of the University of Padua that designs and build high performance small sailing boats used in regattas against other universities.
The goal of the project is to collect data (e.g. wind speed, boat speed, boat direction,...) through several sensors placed in the boat in order to:

* Store them in a database for later analysis
* Show them to the crew through an onboard display
* Transmit them to the coach boat or to the ground station for real-time control and monitoring

The system is structured in modules, connected to each other via Wi-Fi, and communicating through a publish-subscribe messaging protocol, namely, MQTT.

<p align="center">
  <img src="Graphics/Modules Diagram.png" width="500">
</p>


## Data Collection Architecture

The following tools and protocols have been used in order to collect and monitor the measurements:

- [MQTT](https://mqtt.org): messaging protocol used to communicate between modules over WiFi using the publish-subscribe pattern. The lightness, speed and ease of use of the protocol determined its choice.
- [Telegraf](https://www.influxdata.com/time-series-platform/telegraf/): tool used to collect metrics from different sources (e.g. MQTT messages) and store them in several possible ways (e.g. in a database). It's part of the InfluxData TICK Stack, therefore it's easily configurable to work with the InfluxDB database.
- [InfluxDB](https://www.influxdata.com/products/influxdb/): time-series database used to store measurements, logs, computed and raw data. It's one of the leading platforms for time-series application and it's highly optimized for this kind of use case.
- [Grafana](https://grafana.com): modular visualization tool that can be connected to a variety of data sources (included InfluxDB) and generates graphs, maps, and plots. It is possible to build highly customized dashboards for every kind of application scenario.

![data-collection-architecture](Graphics/Data%20Acquisition%20Diagram.png)

## Modules Documentation

The following are the modules in current developement, click on the links to get more detailed information:
* [SailTrack Core](https://github.com/metis-vela-unipd/sailtrack-documentation/tree/main/SailTrack%20Core): central module, it manages connections and gathers data.
* [SailTrack Radio](https://github.com/metis-vela-unipd/sailtrack-documentation/tree/main/SailTrack%20Radio): module for getting GPS data and for transmitting data to the ground base station.
* [SailTrack Monitor](https://github.com/metis-vela-unipd/sailtrack-documentation/tree/main/SailTrack%20Monitor): on board monitor for visualizing real time data for the crew.
* [SailTrack Strain](https://github.com/metis-vela-unipd/sailtrack-documentation/tree/main/SailTrack%20Strain): module for measuring the forces acting on the boat maneuvers.
* [SailTrack Wind](https://github.com/metis-vela-unipd/sailtrack-documentation/tree/main/SailTrack%20Wind): module for getting wind data, such as direction and intensity.
* [SailTrack IMU](https://github.com/metis-vela-unipd/sailtrack-documentation/tree/main/SailTrack%20IMU): module for getting combined orientation and acceleration data of the boat.
