# SailTrack Core
Central module of the SailTrack system, it manages connections and gathers data.

## Hardware Architecture
<p align="center">
  <img src="block-diagram.svg"/>
</p>

## Software Architecture [DRAFT]
The software is structured in services and tasks. Each task is represented by a Python script that runs in a standalone process, and each service is a unit service managed by `systemd`. All the services are grouped under a single, unique, root service.
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

### Resources
* [Bill Of Materials](BOM.csv)
* [Code Repository](https://github.com/metis-vela-unipd/sailtrack-core)
