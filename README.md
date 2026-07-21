# F1SIXTH

A one-sixth-scale autonomous driving research platform based on the Traxxas X-Maxx chassis.

This repository provides the 3D-printable CAD files and supporting information associated with the following paper:

> **A Small-Scale Robot for Autonomous Driving: Design, Challenges, and Best Practices**  
> Hossein Maghsoumi and Yaser Fallah  
> *2025 IEEE 102nd Vehicular Technology Conference (VTC2025-Fall)*, pp. 1–6.

## Overview

F1SIXTH is a small-scale autonomous vehicle platform designed for research in autonomous driving, connected and cooperative vehicles, trajectory tracking, and vehicle control.

Compared with smaller platforms such as F1TENTH, the one-sixth-scale platform offers:

- Higher payload capacity
- More space for onboard computing and sensors
- Longer battery operation
- Improved mechanical stability
- Vehicle dynamics that more closely approximate a full-size vehicle

The platform can accommodate components such as an NVIDIA Jetson computer, Pixhawk autopilot, RTK-GNSS receiver, telemetry radio, cameras, LiDAR, and wireless communication modules.

## Repository Contents

```text
F1SIXTH/
├── CAD/
│   ├── Main_Holder.stl
│   └── Optional_Extension_Module.stl
├── README.md
├── LICENSE
└── CITATION.cff
```

### CAD Files

- `CAD/Main_Holder.stl`  
  Main electronics holder designed for mounting onboard computing, autopilot, positioning, and communication components.

- `CAD/Optional_Extension_Module.stl`  
  Optional extension module that supports alternative placement of the autopilot, GNSS receiver, or other hardware.

Before printing, verify the model dimensions, mounting-hole locations, printer tolerances, and compatibility with your vehicle configuration.

## Recommended Platform Upgrades

Based on our experimental experience, the following mechanical upgrades can improve durability and steering performance:

- High-torque digital steering servo
- Aluminum steering assembly
- Adjustable steering links
- Hardened metal pinion and spur gears
- Upgraded servo saver spring

The paper also discusses recommended PX4 and corresponding ArduPilot parameters for speed control, throttle limits, wheelbase configuration, GPS communication, MAVLink communication, and steering and throttle outputs.

## Paper

The paper presents:

- Mechanical and electronic system design
- Hardware and software integration
- Common mechanical challenges and practical solutions
- Custom electronics-holder design
- PX4 and ArduPilot configuration guidance
- Recommended component upgrades
- Closed-loop trajectory-tracking experiments
- Cooperative driving experiments with three vehicles

An open-access preprint is available on arXiv:

https://arxiv.org/abs/2506.15870

## Citation

Please cite the following paper when using the designs or materials in this repository:

```bibtex
@inproceedings{maghsoumi2025f1sixth,
  author    = {Hossein Maghsoumi and Yaser Fallah},
  title     = {A Small-Scale Robot for Autonomous Driving: Design, Challenges, and Best Practices},
  booktitle = {2025 IEEE 102nd Vehicular Technology Conference (VTC2025-Fall)},
  pages     = {1--6},
  year      = {2025},
  publisher = {IEEE}
}
```

Citation metadata is also provided in `CITATION.cff`.

## Authors

**Hossein Maghsoumi**  
**Yaser Fallah**

Department of Electrical and Computer Engineering  
University of Central Florida  
Orlando, Florida, USA
