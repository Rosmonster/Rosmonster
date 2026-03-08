# 👋 Hello

Bridging the Sim-to-Real gap by deploying VLA and Reinforcement Learning to build robust, intelligent robots for everyday life

🚀 Focused on: Sim-to-Real Transfer | VLA Models | Robot Learning

## 🛠 Skills & Tools

### 🤖 Robotics & AI
![ROS 2](https://img.shields.io/badge/ROS2-22314E?style=for-the-badge&logo=ros&logoColor=white)
![Isaac Sim](https://img.shields.io/badge/Isaac_Sim-76B900?style=for-the-badge&logo=nvidia&logoColor=white)
![Reinforcement Learning](https://img.shields.io/badge/Reinforcement_Learning-FF6F00?style=for-the-badge)

### 💻 Languages & Development
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)

## 🚀 Projects
### 1. 🤖 DolbotX (다목적 임무 수행 로봇 / Multi-purpose Mission Robot)
- **Description:** 
  - 🇰🇷 험지 극복, 물체 추적, 비전 인식 및 로봇팔 피킹 기능을 갖춘 ROS2 기반의 다목적 자율 주행 로봇 개발
  - 🇬🇧 Developed a ROS2-based multi-purpose autonomous robot capable of overcoming rough terrain, object tracking, vision recognition, and robotic arm picking.
- **Roles & Features:**
  - 🇰🇷 임무 수행을 위한 6자유도(6DOF) 커스텀 로봇 팔 기구부 설계 및 자체 제작
  - 🇬🇧 Designed and fabricated a custom 6-DOF robotic arm hardware for mission execution.
  - 🇰🇷 험지 환경에서의 주행 제어 및 극복 알고리즘 구현
  - 🇬🇧 Implemented driving control and overcoming algorithms in rough terrain environments.
  - 🇰🇷 비전 인식 기반의 물체 탐지 및 실시간 타겟 추적
  - 🇬🇧 Real-time target tracking and object detection based on vision recognition.
  - 🇰🇷 파악 대상 인지 후 로봇팔을 이용한 정밀 피킹 작업 수행
  - 🇬🇧 Precise picking operation using a robotic arm after recognizing the target object.
- **Tech Stack:** 
  - `ROS2` `Python` `C++` `Moveit 2` `MTC` (Software)
  - `NVIDIA Jetson` `Arduino` `OpenCR` `CAD / 3D Printing` (Hardware & Embedded)
- **Link:** [GitHub 레포지토리 링크 - 추가 필요]
- <img src="https://github.com/Rosmonster/Rosmonster/issues/1#issue-4040703925" width="600" />

### 2. 🦽 음성 제어 전동 휠체어 시스템 (Voice-Controlled Autonomous Wheelchair)
- **Description:** 
  - 🇰🇷 전신마비 장애인의 자율적인 이동을 지원하는 ROS 2 기반 음성 제어 전동휠체어 시스템 개발
  - 🇬🇧 Developed a ROS 2-based voice-controlled autonomous wheelchair system to support the autonomous mobility of paralyzed individuals.
- **Roles & Features:**
  - 🇰🇷 STT -> LLM -> Nav2 -> Action으로 이어지는 파이프라인 통합 제어 체계 구축
  - 🇬🇧 Built an integrated control pipeline connecting STT, LLM, Nav2, and Action.
  - 🇰🇷 Wheel encoder, 2D LiDAR, IMU 데이터를 융합한 SLAM 기반의 고정밀 환경 지도 작성 및 실시간 위치 추정 기술 구현
  - 🇬🇧 Implemented high-precision mapping and real-time state estimation utilizing SLAM by fusing Wheel encoder, 2D LiDAR, and IMU sensor data.
  - 🇰🇷 Nav2 프레임워크 내 MPPI 컨트롤러를 적용하여 동적 장애물에 대응하는 최적 경로 생성 및 부드러운 주행 제어 성능 확보
  - 🇬🇧 Deployed an MPPI (Model Predictive Path Integral) controller within the Nav2 framework for optimal trajectory generation and smooth obstacle avoidance in dynamic environments.
- **Tech Stack:** 
  - `ROS 2` `Python` `Nav2` `SLAM`
  - `STT` `LLM`
  - `Depth Camera` `2D LiDAR` `IMU`
  - `Hardware Design`
- **Link:** [GitHub 레포지토리 링크 - 추가 필요]

### 3. 🤖 SmolVLA 기반 로봇 팔 제어 및 시뮬레이션 파이프라인 (SmolVLA-Gazebo Integration Pipeline)
- **Description:** 
  - 🇰🇷 최신 Vision-Language-Action (SmolVLA) 모델을 커스텀 로봇 팔에 적용하기 위한 시뮬레이션 기반 학습 및 테스트 환경 구축
  - 🇬🇧 Built a simulation-based training and testing environment to integrate a state-of-the-art VLA model (SmolVLA) with a custom robotic arm.
- **Roles & Features:**
  - 🇰🇷 [Data Generation] MoveIt과 RViz 인터페이스를 활용하여 로봇 팔의 시각-행동(Vision-Action) 궤적 데이터를 직접 생성하고 학습용 데이터셋 구축
  - 🇬🇧 Generated vision-action trajectory data and built a custom training dataset utilizing MoveIt and the RViz interface.
  - 🇰🇷 [Pipeline Setup] SmolVLA 모델과 Gazebo 시뮬레이터를 연동하여 이미지 데이터 수집 및 액션 명령을 주고받는 전체 추론 루프(Inference Loop) 설계
  - 🇬🇧 Designed an end-to-end inference loop connecting the SmolVLA model with Gazebo to stream image data and execute action commands.
  - 🇰🇷 [Task Adaptation] 물리 엔진의 접촉(Contact) 시뮬레이션 불안정성을 고려하여, 파지(Grasping) 대신 물체 집기 직전까지의 '목표 객체 도달(Pre-grasp Reaching)' 모션으로 태스크를 재정의하여 모델 성능 검증
  - 🇬🇧 Redefined the task to 'pre-grasp reaching' to validate the model's spatial reasoning, deliberately avoiding the simulator's unstable contact dynamics during full grasping.
- **Troubleshooting & Future Work:**
  - 🇰🇷 현재 파이프라인 상의 추론 오차(이미지 전송 손실, 학습 데이터셋 편향성 등) 원인 분석 및 모델 최적화 방향 모색
  - 🇬🇧 Analyzing inference errors (e.g., image transmission loss, training data bias) to optimize the model and improve the success rate of the reaching task.
- **Tech Stack:** 
  - `SmolVLA` `ROS 2` `Gazebo` `MoveIt` `RViz` `Python`
- **Link:** [GitHub 레포지토리 링크 - 추가 필요]

### 4. 🦾 로봇 팔 기반 주조품 디버링 자동화 파이프라인 (Automated Robotic Deburring Pipeline)
- **Description:** 
  - 🇰🇷 Vision AI와 시뮬레이션 합성 데이터를 활용한 6축 로봇 팔 디버링(Deburring) 자동화 및 통합 제어 파이프라인 구축 
  - 🇬🇧 Built an automated 6-axis robotic deburring and integrated control pipeline utilizing Vision AI and simulation-based synthetic data.
- **Roles & Features:**
  - 🇰🇷 [Synthetic Data Generation] Isaac Sim을 활용하여 정상 주조품 3D 모델에 무작위 버(Burr)를 생성하고, 2D 카메라 렌더링을 통해 Vision 모델 학습용 대규모 합성 데이터 구축
  - 🇬🇧 Generated large-scale synthetic data for Vision AI training by simulating randomized burrs on normal casted parts and rendering 2D camera images within Isaac Sim.
  - 🇰🇷 [Vision AI & Perception] 구축한 합성 데이터로 IS-Net을 학습시켜 주조품의 버 경계를 정밀하게 추출하고 크기를 분석 (OpenCV 연동)
  - 🇬🇧 Trained IS-Net with the synthetic dataset to accurately extract burr boundaries and analyze their sizes, integrated with OpenCV.
  - 🇰🇷 [Adaptive Path Planning] MoveIt 2를 활용하여 디버링 웨이포인트(Waypoint)를 생성하고, 인식된 버의 크기에 비례하여 로봇 팔의 궤적 이동 속도를 조절하는 가변 속도 제어(Variable Speed Control) 알고리즘 구현
  - 🇬🇧 Developed a variable speed control algorithm and generated waypoints using MoveIt 2, dynamically adjusting the robot arm's trajectory speed based on the analyzed burr size.
  - 🇰🇷 [Sim-to-Real Validation] 실제 가공(Real Machining) 전 단계로서, Isaac Sim 환경 내에서 로봇 팔의 웨이포인트 추종 및 디버링 궤적 검증 수행
  - 🇬🇧 Validated the waypoint tracking and deburring trajectories within the Isaac Sim environment as a crucial pre-requisite for real-world physical machining.
- **Current Status & Future Work:**
  - 🇰🇷 인지(IS-Net)부터 제어(MoveIt 2), 검증(Isaac Sim)까지 이어지는 개별 모듈의 Sim-to-Real 통합 파이프라인 구축 및 최적화 진행 중
  - 🇬🇧 Currently integrating and optimizing the end-to-end Sim-to-Real pipeline, connecting perception (IS-Net), control (MoveIt 2), and simulation validation (Isaac Sim).
- **Tech Stack:** 
  - `ROS 2` `MoveIt 2` `Isaac Sim` `IS-Net` `OpenCV` `Python`
- **Link:** [GitHub 레포지토리 링크 - 추가 필요]

## 📫 Contact Me
- **Email:** [이메일 주소]
- **Blog / Portfolio:** [블로그나 포트폴리오 주소]
