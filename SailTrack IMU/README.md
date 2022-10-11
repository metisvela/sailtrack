# SailTrack IMU
The SailTrack IMU module contains the Inertial Measurement Unit (IMU) sensor to provide attitude information about the boat, such as heading, pitch, roll,... The module is based on an ESP32 microcontroller, that connects to the SailTrack Network to exchange MQTT messages containing the readings of the sensor.

The module performs the following tasks:

* It gets accelerometer, gyroscope and magnetometer data coming from the on-board sensors.
* If fuses raw data using a Kalman filter in order to obtain attitude information of the boat (heading, pitch, roll,...).

The module is mounted in a waterproof enclosure and it is placed at the bottom of the mast, as close as possible to the center of rotation of the boat.

![imu-image](Assets/IMU%20Image.jpg)

## Resources
* [Module Repository](https://github.com/metis-vela-unipd/sailtrack-imu)
