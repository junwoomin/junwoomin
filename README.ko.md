# 전우민 · Woomin Jun

[English](README.md) · **한국어**

자율주행 AI · BEV 인지 · 강화학습 · NPU 커널 최적화

효율적인 인지 모델, 시뮬레이션과 데이터 생성, 주행 정책, 자원이 제한된 하드웨어에서의 배포를 연구합니다.

**포트폴리오** · [English](https://github.com/junwoomin/portfolio) · [한국어](https://github.com/junwoomin/portfolio/blob/main/README_ko.md)  
**이메일** · [kpwoomin@gmail.com](mailto:kpwoomin@gmail.com)

[![LinkedIn](assets/linkedin.svg)](https://www.linkedin.com/in/%EC%9A%B0%EB%AF%BC-%EC%A0%84-61277b372/)

## 대표 논문

- **[SAFE-Q: Safety-Aware End-to-End Driving Using CrossQ Deep Reinforcement Learning](https://doi.org/10.1109/JSEN.2025.3633658)**  
  Yechan Park†, **Woomin Jun†**, Sungjin Lee · *IEEE Sensors Journal*, 26(2), 2848–2855, 2026.  
  멀티태스크 인지, 안전을 고려한 지역 경유점, CrossQ 기반 주행 제어를 통합하고 CARLA에서 평가했습니다.

- **[Synthetic Data Enhancement and Network Compression Technology of Monocular Depth Estimation for Real-Time Autonomous Driving System](https://doi.org/10.3390/s24134205)**  
  **Woomin Jun**, Jisang Yoo, Sungjin Lee · *Sensors*, 24(13), 4205, 2024.  
  단안 깊이 추정을 위한 합성 데이터 증강과 모델 압축을 연구하고, NVIDIA Jetson AGX Orin에서 배포 성능을 평가했습니다.

- **[Optimal Configuration of Multi-Task Learning for Autonomous Driving](https://doi.org/10.3390/s23249729)**  
  **Woomin Jun**, Minjun Son, Jisang Yoo, Sungjin Lee · *Sensors*, 23(24), 9729, 2023.  
  인지 정확도, 지연시간, 모델 크기를 함께 고려한 멀티태스크 구성과 최적화를 연구했습니다.

† 공동 제1저자.

## 대표 프로젝트

| 프로젝트 | 수행 내용 및 근거 | 현재 단계 / 다음 과제 |
| --- | --- | --- |
| **[Tenstorrent P100a](https://github.com/junwoomin/tenstorrent_p100a_project)** | VGG11으로 기본 TTNN 구성과 튜닝을 확인한 뒤, TT-Metalium을 사용해 ResNet bottleneck 전용 커널을 개발했습니다. | 커널 개발 및 실험 기록 정리. |
| **[HBLR](https://github.com/junwoomin/HBLR)** | CARLA BEV 정답 데이터의 차선, 주행 가능 영역, 도로 높이 오류를 분석하고 수정했습니다. [구현 코드](https://github.com/SungjinDavidLee/AGILEQ-Training/tree/main/data_gen). | 시각적 비교와 기술 분석을 포함한 연구 모듈. |
| **[SDV](https://github.com/junwoomin/SDV)** | 센서 설정 → 데이터 수집 → 모델 학습 → 결과 확인을 지원하는 CARLA 실험 UI입니다. 개발 당시 기본 흐름이 동작했습니다. [UI 시연](https://youtu.be/Y6UTaquOltg) · [FMTC 지도 / LiDAR 4대 시연](https://youtu.be/UsxVp50MeAM). | 개발 당시 동작한 프로토타입으로, 재현성과 실험 통합을 개선할 계획입니다. |
| **[LRS — Low Resource Simulation](https://github.com/junwoomin/LRS)** | 차량 동역학, 공유 강화학습 정책을 통한 NPC 제어, 다중 차량 데이터 수집, 실험적인 PPO 학습 흐름을 갖춘 경량 2D BEV 시뮬레이터입니다. | 개발 당시 기본 흐름이 동작했으며, 학습 성능과 데이터 추출 처리량 개선이 남아 있습니다. |
| **[실차 통합](https://github.com/junwoomin/portfolio/blob/main/docs/projects.md)** | ERP42 하드웨어·소프트웨어 통합, RS232 통신, ROS 제어, 카메라 기반 차선 유지, 멀티태스크 인지, 3D SLAM을 구현·통합했습니다. | 실차 시연: [차선 유지](https://youtu.be/_pjnSMG2kxE) · [인지 / SLAM](https://youtu.be/ng5Ybwfu_Hg). |

SDV는 KETI에서 수석연구원의 제안을 계기로 약 3개월 동안 독립적으로 개발했습니다. 정식 연구 과제가 아닌 탐색적 프로토타입이었으며, KETI를 떠나면서 개발을 중단했습니다. 현재 공개된 SDV와 LRS 버전에서 개발 당시의 흐름을 재현하려면 추가 정비가 필요합니다.

## 다음 개발 과제

- **LRS:** 다중 차량 데이터 추출 시 발생하는 틱당 처리 지연을 줄이고, 정책 학습 성능을 개선하며, 시뮬레이션 및 데이터 수집 처리량을 측정합니다.
- **SDV:** 기본 실험 흐름을 재현 가능하게 정비하고, LRS 및 FMTC CARLA 지도와의 연동을 강화합니다. 실제 데이터나 다른 시뮬레이터의 스타일을 활용하는 UniScene 기반 아이디어를 참고해 스타일 전이와 데이터 증강을 탐색하고, 후속으로 CARLA 검증과 강건성 평가를 진행할 계획입니다.

[더 많은 프로젝트, 시연 및 연구 배경 →](https://github.com/junwoomin/portfolio/blob/main/README_ko.md)
