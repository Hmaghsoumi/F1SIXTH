# F1SIXTH

A one-sixth-scale autonomous driving research platform based on the
Traxxas X-Maxx chassis.

This repository provides the CAD files and supplementary materials for
the paper:

> **A Small-Scale Robot for Autonomous Driving: Design, Challenges, and Best Practices**  
> Hossein Maghsoumi and Yaser Fallah  
> *2025 IEEE 102nd Vehicular Technology Conference (VTC2025-Fall)*, pp. 1–6.

## Overview

F1SIXTH is a small-scale autonomous vehicle platform designed for
research in autonomous driving, connected vehicles, trajectory tracking,
and cooperative driving.

Compared with smaller platforms such as F1TENTH, the one-sixth-scale
platform provides:

- Higher payload capacity
- Longer battery operation
- More realistic vehicle dynamics
- Additional space for sensors and onboard computing
- Support for NVIDIA Jetson, Pixhawk, RTK-GNSS, cameras, and LiDAR

## Platform Components

The platform may include:

- Traxxas X-Maxx chassis
- NVIDIA Jetson AGX Xavier
- Pixhawk autopilot
- F9P RTK-GNSS
- SiK telemetry radio
- Wi-Fi communication modules
- LiPo batteries
- Custom 3D-printed electronics holder

## CAD Files

The following 3D-printable models are provided in the `CAD` directory:

- `Main_Holder.stl` — Main holder for onboard electronics
- `Optional_Extension_Module.stl` — Optional module for alternative
  sensor or autopilot placement

## Recommended Mechanical Upgrades

Based on our experimental experience, the following upgrades are
recommended:

- High-torque digital steering servo
- Aluminum steering assembly
- Adjustable steering links
- Hardened metal pinion and spur gears
- Upgraded servo saver spring

## Firmware Configuration

The paper provides recommended PX4 and corresponding ArduPilot parameters
for:

- Ground-speed control
- Throttle limits
- Wheelbase configuration
- GPS communication
- MAVLink communication
- Steering and throttle PWM outputs

Detailed configuration information will be included in the `docs`
directory.

## Paper

The paper describes:

- Mechanical and electronic system design
- Hardware integration
- Common mechanical challenges and solutions
- Custom holder design
- PX4 and ArduPilot parameter configuration
- Recommended component upgrades
- Closed-loop trajectory-tracking experiments
- Three-vehicle cooperative driving experiments

## Citation

Please cite the following paper when using this repository:

```bibtex
@inproceedings{maghsoumi2025f1sixth,
  title={A Small-Scale Robot for Autonomous Driving: Design, Challenges, and Best Practices},
  author={Maghsoumi, Hossein and Fallah, Yaser},
  booktitle={2025 IEEE 102nd Vehicular Technology Conference (VTC2025-Fall)},
  pages={1--6},
  year={2025},
  organization={IEEE}
}
