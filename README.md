# Awesome Embodied AI for Earth / 具身智能 × 地球·水文

> Curated **Embodied AI** papers, code, simulators & benchmarks — with **extra focus on Earth / hydrology applications** (underwater & marine robots, construction & infrastructure robots, disaster prevention & response, environmental / hydrological monitoring).

> 收录具身智能（Embodied AI）代表性工作，并**着重**地球科学 / 水文相关应用：水下与海洋机器人、建筑与基础设施机器人、灾害防治与应急、环境与水文监测。

**Last updated:** 2026-11-05 (Asia/Shanghai)

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

## Earth & Hydrology Applications / 地球与水文科学应用

> This section is the **priority growth area** of the list. Contributions especially welcome.

### Underwater & Marine / 水下与海洋

- **Deep Learning for Visual Navigation of Underwater Robots** (2023) [[arXiv](https://arxiv.org/abs/2310.19495)] — _Survey of DL visual navigation for AUVs._
- **Sonar-based Deep Learning in Underwater Robotics** (2024) [[arXiv](https://arxiv.org/abs/2412.11840)] — _Sonar DL tasks, datasets, simulators, robustness._
- **BlueOS** — [[GitHub](https://github.com/bluerobotics/BlueOS)] — _Open platform for ROV / USV / robotic system ops (Blue Robotics)._
- **UUV Simulator** — [[GitHub](https://github.com/uuvsimulator/uuv_simulator)] — _Classic Gazebo underwater robot simulation._
- **BRUCE (BlueRov Underwater SLAM and Exploration)** — [[GitHub](https://github.com/jinkunw/bruce)] — _BlueROV SLAM / exploration codebase._

### Construction & Infrastructure / 建筑与基础设施

- **Navigation2** — [[GitHub](https://github.com/ros-navigation/navigation2)] — _ROS 2 navigation stack widely used for mobile inspection robots._
- **PX4 Autopilot** — [[GitHub](https://github.com/PX4/PX4-Autopilot)] — _Open autopilot for drones used in infrastructure inspection._
- **mav_voxblox_planning** — [[GitHub](https://github.com/ethz-asl/mav_voxblox_planning)] — _MAV planning with voxblox maps (inspection / mapping)._
- *More construction-robot learning papers will be added in the next refresh cycles.*

### Disaster Prevention & Response / 灾害防治与应急

- **Deep Learning for Rapid Landslide Detection using SAR Datacubes** (2022) [[arXiv](https://arxiv.org/abs/2211.02869)] [[Code](https://github.com/iprapas/landslide-sar-unet)] — _Sentinel-1 SAR → landslide segmentation (emergency mapping)._
- **A Survey on Unmanned Surface Vehicles for Disaster Robotics** (2019) [[MDPI Sensors](https://www.mdpi.com/1424-8220/19/3/702)] — _USV roles in disaster scenarios incl. flood/landslide sensing._
- **Artificial intelligence based framework for robotic search and rescue operations conducted jointly by international teams** — Magid et al. (2020) [[DOI](https://doi.org/10.1007/978-981-13-9267-2_2)] — _Heterogeneous UAV/UGV/USV/UUV teams for flood & landslide sites._
- **RoboCup Rescue Simulator** — [[GitHub](https://github.com/roborescue/rcrs-server)] — _Standardized disaster-response robotics simulation._

### Environmental & Hydrological Monitoring / 环境与水文监测

- **Virtual RobotX (VRX)** — [[GitHub](https://github.com/osrf/vrx)] — _Surface autonomy tasks relevant to coastal / harbor monitoring._
- **BlueOS** — [[GitHub](https://github.com/bluerobotics/BlueOS)] — _Payload ops for ROV/USV monitoring platforms._
- *Hydrology-specific USV / reservoir / water-quality robot papers are prioritized for upcoming updates.*

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
