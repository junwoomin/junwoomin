# Woomin Jun

**English** · [한국어](README.ko.md)

Autonomous Driving AI · BEV Perception · Reinforcement Learning · NPU Kernel Optimization

I work on efficient perception, simulation and data generation, driving policies, and deployment on constrained hardware.

**Portfolio** · [English](https://github.com/junwoomin/portfolio) · [한국어](https://github.com/junwoomin/portfolio/blob/main/README_ko.md)  
**Email** · [kpwoomin@gmail.com](mailto:kpwoomin@gmail.com)

[![LinkedIn](assets/linkedin.svg)](https://www.linkedin.com/in/%EC%9A%B0%EB%AF%BC-%EC%A0%84-61277b372/)

## Selected Publications

- **[SAFE-Q: Safety-Aware End-to-End Driving Using CrossQ Deep Reinforcement Learning](https://doi.org/10.1109/JSEN.2025.3633658)**  
  Yechan Park†, **Woomin Jun†**, Sungjin Lee · *IEEE Sensors Journal*, 26(2), 2848–2855, 2026.  
  Multi-task perception, safety-aware local waypoints, and CrossQ-based driving control evaluated in CARLA.  
  [Training code](https://github.com/SungjinDavidLee/AGILEQ-Training) · [Evaluation code](https://github.com/SungjinDavidLee/AGILEQ-Evaluation)

- **[Synthetic Data Enhancement and Network Compression Technology of Monocular Depth Estimation for Real-Time Autonomous Driving System](https://doi.org/10.3390/s24134205)**  
  **Woomin Jun**, Jisang Yoo, Sungjin Lee · *Sensors*, 24(13), 4205, 2024.  
  Synthetic data augmentation and model compression for monocular depth estimation, with deployment evaluation on NVIDIA Jetson AGX Orin.

- **[Optimal Configuration of Multi-Task Learning for Autonomous Driving](https://doi.org/10.3390/s23249729)**  
  **Woomin Jun**, Minjun Son, Jisang Yoo, Sungjin Lee · *Sensors*, 23(24), 9729, 2023.  
  Multi-task configuration and optimization balancing perception accuracy, latency, and model size.

† Equal contribution.

## Selected Projects

| Project | Work and evidence | Stage / next focus |
| --- | --- | --- |
| **[Tenstorrent P100a](https://github.com/junwoomin/tenstorrent_p100a_project)** | TTNN VGG11 configuration and tuning, followed by dedicated ResNet bottleneck kernels using TT-Metalium. | Kernel development and experiment records. |
| **[HBLR](https://github.com/junwoomin/HBLR)** | Analysis and correction of CARLA BEV ground-truth errors in lane markings, drivable areas, and road elevation. [Implementation](https://github.com/SungjinDavidLee/AGILEQ-Training/tree/main/data_gen). | Research module with visual comparisons and technical analysis. |
| **[SDV](https://github.com/junwoomin/SDV)** | CARLA experiment UI for sensor configuration → data collection → model training → result inspection. The basic workflow ran during development. [UI demo](https://youtu.be/Y6UTaquOltg) · [FMTC map / four-LiDAR demo](https://youtu.be/UsxVp50MeAM). | Working prototype during development; further work planned on reproducibility and experiment integration. |
| **[LRS — Low Resource Simulation](https://github.com/junwoomin/LRS)** | Lightweight 2D BEV simulation with vehicle dynamics, shared RL policy control of NPCs, multi-vehicle data collection, and an experimental PPO workflow. | Basic workflow ran during development; learning performance and data extraction throughput remain improvement priorities. |
| **[Real-Vehicle Integration](https://github.com/junwoomin/portfolio/blob/main/docs/projects.md)** | ERP42 hardware/software integration, RS232 communication, ROS control, camera-based lane keeping, multi-task perception, and 3D SLAM. | Vehicle demonstrations: [lane keeping](https://youtu.be/_pjnSMG2kxE) · [perception / SLAM](https://youtu.be/ng5Ybwfu_Hg). |

SDV was independently developed over approximately three months at KETI, following a senior principal researcher's suggestion. It was an exploratory prototype rather than a formal research project; development paused when I left KETI. The current public SDV and LRS snapshots still need work to reproduce the original development workflows.

## Next Development Priorities

- **LRS:** reduce per-tick overhead when extracting data from multiple vehicles, improve policy learning, and benchmark simulation and collection throughput.
- **SDV:** make the basic experiment workflow reproducible, strengthen integration with LRS and the FMTC CARLA map, and explore UniScene-inspired style transfer and data augmentation using real data or other simulator styles. CARLA validation and robustness evaluation are planned follow-up work.

[More projects, demonstrations, and research background →](https://github.com/junwoomin/portfolio)
