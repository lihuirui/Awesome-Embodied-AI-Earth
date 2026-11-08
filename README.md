# Awesome Embodied AI for Earth / 具身智能 × 地球·水文

> Curated **Embodied AI** papers, code, simulators & benchmarks — with **extra focus on Earth / hydrology applications** (underwater & marine robots, construction & infrastructure robots, disaster prevention & response, environmental / hydrological monitoring).

> 收录具身智能（Embodied AI）代表性工作，并**着重**地球科学 / 水文相关应用：水下与海洋机器人、建筑与基础设施机器人、灾害防治与应急、环境与水文监测。

**Last updated:** 2026-11-08 (Asia/Shanghai)

**Rules:** only verified links (arXiv / GitHub / publisher). Do **not** invent titles, IDs, or stars. Seed list in [`data/papers.json`](data/papers.json).

## Table of Contents

- [Surveys / 综述](#surveys--综述)
- [Foundation Embodied AI / 具身智能基础](#foundation-embodied-ai--具身智能基础)
- [Simulators & Benchmarks / 仿真与基准](#simulators--benchmarks--仿真与基准)
- [Earth & Hydrology Applications / 地球与水文科学应用](#earth--hydrology-applications--地球与水文科学应用)
  - [Underwater & Marine / 水下与海洋](#underwater--marine--水下与海洋)
  - [Construction & Infrastructure / 建筑与基础设施](#construction--infrastructure--建筑与基础设施)
  - [Disaster Prevention & Response / 灾害防治与应急](#disaster-prevention--response--灾害防治与应急)
  - [Environmental & Hydrological Monitoring / 环境与水文监测](#environmental--hydrological-monitoring--环境与水文监测)
- [Datasets / 数据集](#datasets--数据集)
- [Toolkits & Resources / 工具与资源](#toolkits--resources--工具与资源)
- [Related Awesome Lists / 相关列表](#related-awesome-lists--相关列表)
- [Maintenance](#maintenance)

---

## Surveys / 综述

- **A Survey on Vision-Language-Action Models for Embodied AI** — Yueen Ma et al. (2024) [[arXiv](https://arxiv.org/abs/2405.14093)] [[Code](https://github.com/yueen-ma/Awesome-VLA)] *(TNNLS 2025)* — _First dedicated VLA survey + taxonomy._
- **Vision-Language-Action Models for Robotics: A Review Towards Real-World Applications** — Kento Kawaharazuka et al. (2025) [[arXiv](https://arxiv.org/abs/2510.07077)] *(IEEE Access)* — _Full-stack VLA review toward deployment._
- **Aligning Cyber Space with Physical World: A Comprehensive Survey on Embodied AI** — Yang Liu et al. (2024) [[arXiv](https://arxiv.org/abs/2407.06886)] — _Broad embodied AI survey (robots, sims, agents)._
- **Toward General-Purpose Robots via Foundation Models: A Survey and Beyond** — Yafei Hu et al. (2023) [[arXiv](https://arxiv.org/abs/2312.08782)] — _Foundation-model path to generalist robots._
- **Deep Learning for Visual Navigation of Underwater Robots** (2023) [[arXiv](https://arxiv.org/abs/2310.19495)] — _Underwater visual nav: perception, datasets, IL/RL._
- **Sonar-based Deep Learning in Underwater Robotics: Overview, Robustness and Challenges** (2024) [[arXiv](https://arxiv.org/abs/2412.11840)] — _Sonar DL perception/SLAM + robustness gaps._
- **A Survey on Unmanned Surface Vehicles for Disaster Robotics: Main Challenges and Directions** — Jorge et al. (2019) [[MDPI Sensors](https://www.mdpi.com/1424-8220/19/3/702)] — _USVs for disaster robotics (flood/landslide-related sensing)._
- **State-of-the-Art Underwater Vehicles and Technologies Enabling Smart Ocean: Survey and Classifications** — Jiajie Xu et al. (2024) [[arXiv](https://arxiv.org/abs/2412.18667)] — _Survey and taxonomy of ROVs/AUVs/HUVs/USVs and smart-ocean enabling technologies._

## Foundation Embodied AI / 具身智能基础

### Vision-Language-Action (VLA) & generalist policies

- **RT-1: Robotics Transformer for Real-World Control at Scale** — Anthony Brohan et al. (2022) [[arXiv](https://arxiv.org/abs/2212.06817)] — _Early large-scale real-robot transformer policy._
- **RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control** — Brianna Zitkovich et al. (2023) [[arXiv](https://arxiv.org/abs/2307.15818)] — _VLM backbone → robot actions._
- **Open X-Embodiment: Robotic Learning Datasets and RT-X Models** — Abby O'Neill et al. (2023) [[arXiv](https://arxiv.org/abs/2310.08864)] [[Project](https://robotics-transformer-x.github.io/)] — _Cross-embodiment dataset + RT-X._
- **OpenVLA: An Open-Source Vision-Language-Action Model** — Moo Jin Kim et al. (2024) [[arXiv](https://arxiv.org/abs/2406.09246)] [[Code](https://github.com/openvla/openvla)] — _Open 7B-class VLA on OXE._
- **Octo: An Open-Source Generalist Robot Policy** — Octo Model Team et al. (2024) [[arXiv](https://arxiv.org/abs/2405.12213)] [[Code](https://github.com/octo-models/octo)] — _Transformer generalist from mixed robot data._
- **π₀: A Vision-Language-Action Flow Model for General Robot Control** — Physical Intelligence et al. (2024) [[arXiv](https://arxiv.org/abs/2410.24164)] [[Code](https://github.com/Physical-Intelligence/openpi)] — _Flow-matching VLA (openpi)._
- **π₀.₅: a Vision-Language-Action Model with Open-World Generalization** — Physical Intelligence et al. (2025) [[arXiv](https://arxiv.org/abs/2504.16054)] [[Code](https://github.com/Physical-Intelligence/openpi)] — _Open-world generalization follow-up._
- **GR-2: A Generative Video-Language-Action Model with Web-Scale Knowledge for Robot Manipulation** — Chi-Lam Cheang et al. (2024) [[arXiv](https://arxiv.org/abs/2410.06158)] — _Video-language-action generative policy._

### LLM agents / reward / humanoids

- **Do As I Can, Not As I Say: Grounding Language in Robotic Affordances (SayCan)** — Michael Ahn et al. (2022) [[arXiv](https://arxiv.org/abs/2204.01691)] — _LLM planning grounded in affordances._
- **Eureka: Human-Level Reward Design via Coding Large Language Models** — Yecheng Jason Ma et al. (2023) [[arXiv](https://arxiv.org/abs/2310.12931)] — _LLM-written reward functions for robot learning._
- **Humanoid Locomotion as Next Token Prediction** — Ilija Radosavovic et al. (2024) [[arXiv](https://arxiv.org/abs/2402.19469)] — _Humanoid control as sequence modeling._

## Simulators & Benchmarks / 仿真与基准

- **Habitat: A Platform for Embodied AI Research** — Manolis Savva et al. (2019) [[arXiv](https://arxiv.org/abs/1904.01201)] [[Code](https://github.com/facebookresearch/habitat-sim)] — _High-performance indoor embodied sim._
- **Isaac Lab** — [[GitHub](https://github.com/isaac-sim/IsaacLab)] — _Unified robot learning with multi-physics/renderer support._
- **ManiSkill** — [[GitHub](https://github.com/mani-skill/ManiSkill)] — _GPU-parallel manipulation simulator & benchmark._
- **robosuite** — [[GitHub](https://github.com/ARISE-Initiative/robosuite)] — _Modular robot learning simulation framework._
- **MuJoCo** — [[GitHub](https://github.com/google-deepmind/mujoco)] — _General-purpose contact physics engine._
- **AirSim** — [[GitHub](https://github.com/microsoft/AirSim)] — _UE/Unity sim for autonomous vehicles (incl. aerial)._
- **UUV Simulator** — [[GitHub](https://github.com/uuvsimulator/uuv_simulator)] — _Gazebo/ROS packages for underwater robotics simulation._
- **Project DAVE** — [[GitHub](https://github.com/Field-Robotics-Lab/dave)] — _Underwater vehicle simulation stack (Field Robotics Lab)._
- **Virtual RobotX (VRX)** — [[GitHub](https://github.com/osrf/vrx)] — _Surface vessel autonomy competition / sim resources._
- **RoboCup Rescue Simulator** — [[GitHub](https://github.com/roborescue/rcrs-server)] — _Disaster-response multi-agent simulation._
- **AquaWorld: Structure-Consistent Underwater World Generation for Robot Simulation** — Bin Peng et al. (2026) [[arXiv](https://arxiv.org/abs/2609.22670)] — _Language-conditioned underwater world generation that keeps terrain, assets, tasks, and currents consistent for robot sim._

## Earth & Hydrology Applications / 地球与水文科学应用

> This section is the **priority growth area** of the list. Contributions especially welcome.

### Underwater & Marine / 水下与海洋

- **Deep Learning for Visual Navigation of Underwater Robots** (2023) [[arXiv](https://arxiv.org/abs/2310.19495)] — _Survey of DL visual navigation for AUVs._
- **Sonar-based Deep Learning in Underwater Robotics** (2024) [[arXiv](https://arxiv.org/abs/2412.11840)] — _Sonar DL tasks, datasets, simulators, robustness._
- **BlueOS** — [[GitHub](https://github.com/bluerobotics/BlueOS)] — _Open platform for ROV / USV / robotic system ops (Blue Robotics)._
- **UUV Simulator** — [[GitHub](https://github.com/uuvsimulator/uuv_simulator)] — _Classic Gazebo underwater robot simulation._
- **BRUCE (BlueRov Underwater SLAM and Exploration)** — [[GitHub](https://github.com/jinkunw/bruce)] — _BlueROV SLAM / exploration codebase._
- **Embodied at Sea: Imitation Learning for Multi-Task Underwater Manipulation** — Greta Perez-Haiek et al. (2026) [[arXiv](https://arxiv.org/abs/2610.38199)] [[Project](https://lair-research-nyu.github.io/Embodied-at-Sea/)] — _Field underwater manipulation via imitation/VLA (DynamicVLA); 1616 episodes and on-hardware pool rollouts._
- **AquaWAM: A Dynamics-aware World Action Model for Underwater Embodied Agents** — Cunhao Zhu et al. (2026) [[arXiv](https://arxiv.org/abs/2609.33299)] — _World-action model that accounts for underwater passive dynamics (inertia, buoyancy, drag, drift)._
- **AquaBEV-Nav: Learned BEV Occupancy for Underwater Navigation and Exploration** — Trung Tien Dong et al. (2026) [[arXiv](https://arxiv.org/abs/2609.32156)] — _Learned bird's-eye-view occupancy for underwater navigation and exploration._
- **CoralPlan: Observation Skill Selection and Execution for Underwater Robotic Inspection** — Yuer Gao et al. (2026) [[arXiv](https://arxiv.org/abs/2609.31211)] — _Selects and executes observation skills for underwater robotic inspection._

### Construction & Infrastructure / 建筑与基础设施

- **Navigation2** — [[GitHub](https://github.com/ros-navigation/navigation2)] — _ROS 2 navigation stack widely used for mobile inspection robots._
- **PX4 Autopilot** — [[GitHub](https://github.com/PX4/PX4-Autopilot)] — _Open autopilot for drones used in infrastructure inspection._
- **mav_voxblox_planning** — [[GitHub](https://github.com/ethz-asl/mav_voxblox_planning)] — _MAV planning with voxblox maps (inspection / mapping)._
- **Sample-Efficient Robot Skill Learning for Construction Tasks: Benchmarking Hierarchical Reinforcement Learning and Vision-Language-Action VLA Model** — Zhaofeng Hu et al. (2025) [[arXiv](https://arxiv.org/abs/2512.14031)] — _Benchmarks hierarchical RL vs. a VLA model for sample-efficient construction-robot skill learning._
- **Generalizable Skill Learning for Construction Robots with Crowdsourced Natural Language Instructions, Composable Skills Standardization, and Large Language Model** — Hongrui Yu et al. (2025) [[arXiv](https://arxiv.org/abs/2509.02876)] — _LLM + crowdsourced language instructions for generalizable construction-robot skill learning._
- **Learning Interaction-Aware Path Corrections from Unlabeled Trajectories: A LiDAR-Based Sim-to-Real GNN Framework for Construction Robots** — Yilong Chen et al. (2026) [[arXiv](https://arxiv.org/abs/2610.34060)] — _LiDAR GNN sim-to-real framework that learns interaction-aware path corrections for construction robots._
- **BIM-Discrepancy-Driven Active Sensing for Risk-Aware UAV-UGV Navigation** — Hesam Mojtahedi et al. (2025) [[arXiv](https://arxiv.org/abs/2511.14037)] — _Uses BIM discrepancies to drive active sensing for risk-aware UAV-UGV inspection navigation._

### Disaster Prevention & Response / 灾害防治与应急

- **Deep Learning for Rapid Landslide Detection using SAR Datacubes** (2022) [[arXiv](https://arxiv.org/abs/2211.02869)] [[Code](https://github.com/iprapas/landslide-sar-unet)] — _Sentinel-1 SAR → landslide segmentation (emergency mapping)._
- **A Survey on Unmanned Surface Vehicles for Disaster Robotics** (2019) [[MDPI Sensors](https://www.mdpi.com/1424-8220/19/3/702)] — _USV roles in disaster scenarios incl. flood/landslide sensing._
- **Artificial intelligence based framework for robotic search and rescue operations conducted jointly by international teams** — Magid et al. (2020) [[DOI](https://doi.org/10.1007/978-981-13-9267-2_2)] — _Heterogeneous UAV/UGV/USV/UUV teams for flood & landslide sites._
- **RoboCup Rescue Simulator** — [[GitHub](https://github.com/roborescue/rcrs-server)] — _Standardized disaster-response robotics simulation._
- **A Simulation-Grounded Agentic VLM Framework for Wildfire Monitoring and Reporting** — Duowen Chen et al. (2026) [[arXiv](https://arxiv.org/abs/2610.02451)] — _Agentic vision-language framework, grounded in simulation, for wildfire monitoring and reporting._
- **Multi-Agent Reinforcement Learning for Autonomous UAV Exploration in Wildfire Response** — Caden Chandra et al. (2026) [[arXiv](https://arxiv.org/abs/2609.10433)] — _Multi-agent RL for autonomous UAV exploration during wildfire response._
- **D3ARC: Time-Critical Distributed Disaster Detection for Asynchronous Cooperative Multi-Robot Systems** — Nikolaos Koursioumpas et al. (2026) [[arXiv](https://arxiv.org/abs/2609.07350)] — _Time-critical distributed disaster detection for asynchronous cooperative multi-robot teams._

### Environmental & Hydrological Monitoring / 环境与水文监测

- **Virtual RobotX (VRX)** — [[GitHub](https://github.com/osrf/vrx)] — _Surface autonomy tasks relevant to coastal / harbor monitoring._
- **BlueOS** — [[GitHub](https://github.com/bluerobotics/BlueOS)] — _Payload ops for ROV/USV monitoring platforms._
- **Constraint-Driven Multi-USV Coverage Path Generation for Aquatic Environmental Monitoring** — Yo Toyomoto et al. (2024) [[arXiv](https://arxiv.org/abs/2411.00579)] [[DOI](https://doi.org/10.1109/TCST.2025.3572776)] — _Constraint-driven multi-USV coverage planning for aquatic environmental monitoring (IEEE TCST)._
- **Towards Design and Development of a Low-Cost Unmanned Surface Vehicle for Aquaculture Water Quality Monitoring in Shallow Water Environments** — Aiyelari Temilolorun and Yogang Singh (2024) [[arXiv](https://arxiv.org/abs/2410.09513)] — _Low-cost USV design for aquaculture water-quality monitoring in shallow waters._
- **3D Water Quality Mapping using Invariant Extended Kalman Filtering for Underwater Robot Localization** — Kaustubh Joshi et al. (2024) [[arXiv](https://arxiv.org/abs/2409.11578)] — _Underwater-robot localization (invariant EKF) for 3D water-quality mapping in aquaculture settings._
- **High-Resolution Water Sampling via a Solar-Powered Autonomous Surface Vehicle** — Misael Mamani et al. (2025) [[arXiv](https://arxiv.org/abs/2512.09798)] — _Solar-powered ASV that collects high-resolution water samples for environmental monitoring._
- **Active Tracking of Marine Pollution Sources: An Uncertainty-Aware Categorical Bayesian Framework for Unmanned Surface Vehicles** — Song Ma et al. (2025) [[arXiv](https://arxiv.org/abs/2509.20593)] — _Uncertainty-aware Bayesian planner for USVs that actively track marine pollution sources._
- **An Autonomous, 3D Printed, Waterjet-Powered, Open-Source Robotic Trimaran for Environmental Inspection and Monitoring** — Reuben O'Brien et al. (2024) [[arXiv](https://arxiv.org/abs/2610.07398)] [[DOI](https://doi.org/10.1109/IROS58592.2024.10801622)] — _Open-source 3D-printed waterjet trimaran for environmental inspection (IROS 2024; Best Application Paper finalist)._

## Datasets / 数据集

- **Open X-Embodiment (OXE)** — [[arXiv](https://arxiv.org/abs/2310.08864)] [[Project](https://robotics-transformer-x.github.io/)] — _Large multi-robot manipulation corpus for VLA / RT-X._
- **Landslide SAR datacubes** — [[arXiv](https://arxiv.org/abs/2211.02869)] [[Code](https://github.com/iprapas/landslide-sar-unet)] — _ML-ready Sentinel-1 cubes + landslide masks._

## Toolkits & Resources / 工具与资源

- **LeRobot** — [[GitHub](https://github.com/huggingface/lerobot)] — _Accessible end-to-end robot learning toolkit (Hugging Face)._
- **openpi** — [[GitHub](https://github.com/Physical-Intelligence/openpi)] — _Open implementation around π-series VLAs._
- **OpenVLA** — [[GitHub](https://github.com/openvla/openvla)] — _Training / inference for OpenVLA._
- **Octo** — [[GitHub](https://github.com/octo-models/octo)] — _Generalist robot policy codebase._

## Related Awesome Lists / 相关列表

- [yueen-ma/Awesome-VLA](https://github.com/yueen-ma/Awesome-VLA)
- [jonyzhang2023/awesome-embodied-vla-va-vln](https://github.com/jonyzhang2023/awesome-embodied-vla-va-vln)
- [zchoi/Awesome-Embodied-Robotics-and-Agent](https://github.com/zchoi/Awesome-Embodied-Robotics-and-Agent)
- [ChanganVR/awesome-embodied-vision](https://github.com/ChanganVR/awesome-embodied-vision)
- [haoranD/Awesome-Embodied-AI](https://github.com/haoranD/Awesome-Embodied-AI)
- Sibling lists by same maintainer: [awesome-ai-earth-science](https://github.com/lihuirui/awesome-ai-earth-science), [awesome-world-models](https://github.com/lihuirui/awesome-world-models)

## Maintenance

- Initial seed curated 2026-11-05 (manual + verified links; Gemini capacity was limited so first fill used lightweight search).
- Planned cadence: refresh about **every 3 days** — add newly verified arXiv/GitHub items, densify Earth/hydro sections, dedupe by arXiv id / URL.
- PRs welcome — see [CONTRIBUTING.md](CONTRIBUTING.md).
- Refresh 2026-11-08: added 19 verified arXiv entries, focused on Earth/hydro (USV water-quality/monitoring, underwater embodied agents, construction-robot learning, disaster/wildfire robotics).
