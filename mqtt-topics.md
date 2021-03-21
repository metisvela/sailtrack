# MQTT Topics Structure
### [Edit Here](https://tree.nathanfriend.io/?s=(%27options!(%27fancy!true~fullPAh!false~ClingSlash!true)~E(%27E%27sensorDgps0*time9modeG2imu0*At4-w*gyro4acc4mag4J80G*direction2sCn0*loaKdAaDboA9sog*cog*vmg*heading8HsHaHdIsIaIKstAusDcore6-level*7Fenv2radio32monitor383DsCn3DB*%27)~version!%271%27)*D--%20%202*BD3674FxFyFz*5%5Cn6*bAFvolt*7JFcpu82wind9*lA*lon*AatB...CtraiD5-Esource!F*-G*speedH*awI*twJtempKd2B5%01KJIHGFEDCBA98765432-*)
```
.
├── sensor/
│   ├── gps0/
│   │   ├── time
│   │   ├── lat
│   │   ├── lon
│   │   ├── mode
│   │   ├── speed
│   │   └── ...
│   ├── imu0/
│   │   ├── att/
│   │   │   ├── x
│   │   │   ├── y
│   │   │   ├── z
│   │   │   └── w
│   │   ├── gyro/
│   │   │   ├── x
│   │   │   ├── y
│   │   │   └── z
│   │   ├── acc/
│   │   │   ├── x
│   │   │   ├── y
│   │   │   └── z
│   │   ├── mag/
│   │   │   ├── x
│   │   │   ├── y
│   │   │   └── z
│   │   ├── temp
│   │   └── ...
│   ├── wind0/
│   │   ├── speed
│   │   ├── direction
│   │   └── ...
│   ├── strain0/
│   │   ├── load
│   │   └── ...
│   └── ...
├── data/
│   ├── boat/
│   │   ├── lat
│   │   ├── lon
│   │   ├── sog
│   │   ├── cog
│   │   ├── vmg
│   │   ├── heading
│   │   └── ...
│   ├── wind/
│   │   ├── aws
│   │   ├── awa
│   │   ├── awd
│   │   ├── tws
│   │   ├── twa
│   │   ├── twd
│   │   └── ...
│   └── ...
└── status/
    ├── core/
    │   ├── bat/
    │   │   ├── volt
    │   │   └── level
    │   ├── temp/
    │   │   ├── cpu
    │   │   └── env
    │   └── ...
    ├── radio/
    │   ├── bat/
    │   │   └── volt
    │   ├── temp/
    │   │   └── cpu
    │   └── ...
    ├── monitor/
    │   ├── bat/
    │   │   └── volt
    │   ├── temp/
    │   │   └── cpu
    │   └── ...
    ├── wind/
    │   ├── bat/
    │   │   └── volt
    │   └── temp/
    │       └── cpu
    ├── strain/
    │   ├── bat/
    │   │   └── volt
    │   └── temp/
    │       └── cpu
    └── ...
```
