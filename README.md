<p align="center">
  <img src="Design/SailTrack Logo.png">
</p>

<h3 align="center"><i>Sailing Performance Tracker</i></h3>

# SailTrack
SailTrack is a performance tracker for sailing boats.
This system is built by the Métis Vela Unipd team, a student project of the University of Padua that designs and build high performance small sailing boats used in regattas against other universities.
The goal of the project is to collect data (e.g. wind speed, boat speed, boat direction,...) through several sensors placed in the boat in order to:
* Store them in a database for later analysis
* Show them to the crew through an onboard display
* Transmit them to the coach boat or to the ground station for real-time control and monitoring

The system is structured in modules, connected to each other via Wi-Fi, and communicating through a publish-subscribe messaging protocol, namely, MQTT.

<p align="center">
  <img src="https://user-images.githubusercontent.com/27573242/113483138-3df4d380-94a2-11eb-87cc-3695a0de3a96.png"/>
</p>

## Modules Documentation
The following are the modules in current developement, click on the links to get more detailed informations:
* [SailTrack Core](https://github.com/metis-vela-unipd/sailtrack-documentation/tree/main/SailTrack%20Core): central module of the SailTrack system, it manages connections and gathers data.
* [SailTrack Radio](https://github.com/metis-vela-unipd/sailtrack-documentation/tree/main/SailTrack%20Radio): module for getting GPS data and for transmitting data to the ground base station.
* [SailTrack Monitor](https://github.com/metis-vela-unipd/sailtrack-documentation/tree/main/SailTrack%20Monitor): on board monitor for visualizing real time data for the crew.
* [SailTrack Strain](https://github.com/metis-vela-unipd/sailtrack-documentation/tree/main/SailTrack%20Strain): module for measuring the forces acting on the boat maneuvers.
* [SailTrack Wind](https://github.com/metis-vela-unipd/sailtrack-documentation/tree/main/SailTrack%20Wind): module for getting wind data, such as direction and intensity.
