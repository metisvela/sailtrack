# SailTrack Core
Central module of the SailTrack system, it manages connections and gathers data. This module is based on a Raspberry Pi, running the latest version of Raspberry Pi OS.

## Hardware Architecture
<p align="center">
  <img src="block-diagram.svg"/>
</p>

## Software Architecture [DRAFT]
The software is structured in `systemd` services, each one running a Python script.
```
.
└── sailtrack.service
    ├── sailtrack.db.service
    │   └── db.py
    ├── sailtrack.imu.service
    │   └── imu.py
    ├── sailtrack.filter.service
    │   └── filter.py
    └── sailtrack.lora.service
        └── lora.py
```

## Resources
* [Bill Of Materials](BOM.csv)
* [Code Repository](https://github.com/metis-vela-unipd/sailtrack-core)
