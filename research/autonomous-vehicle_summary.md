---
layout: page-wide
title: Autonomous Driving Group
permalink: /research/autonomous-vehicle.html
---





## Introduction

The core focus of our research is to understand the interactive human (driving) behavior and the scene with proper representations, and to predict and emulate the behavior to enable safe and high-quality autonomy for various mobility. Our viewpoint is to exploit the synergies of model-based planning/control methods and state-of-the-art machine learning techniques to combine our prior and what we can learn from data. In order to sufficiently support the focus, our research scope also expands to the fundamental aspects such as validation/evaluation and dataset construction. We also dive into perception from different perspectives and control for various platforms, and incorporate our behavior-related research insights into these aspects.



The group lead is Dr. [Wei Zhan](https://scholar.google.com/citations?user=xVN3UxYAAAAJ&hl=en#). The research activities are conducted by 2 Postdocs (Dr. [Wei Zhan](https://scholar.google.com/citations?user=xVN3UxYAAAAJ&hl=en#) and Dr. [Liting Sun](https://scholar.google.com/citations?user=BitIg-YAAAAJ&hl=en)) and 13 Ph.D. students with over 10 visiting researchers. Our algorithms were tested on autonomous vehicles in test fields supported by our sponsors and collaborators. We collected raw data from onboard sensors (LiDARs/cameras) on our data-collection vehicle and other fixed sensors, as well as behavior data from two sets of driving simulators with mechanical interfaces. Two datasets ([INTERACTION](https://interaction-dataset.com/) and [UrbanLoco](https://advdataset2019.wixsite.com/urbanloco)) were published. Several recent publications on autonomous driving by laboratory members received Best Student Paper or Best Paper Finalist in flagship conferences on robotics and intelligent vehicle/transportation, such as *IROS*, *ITSC* and *IV*.



## Research Topics



### 1. Prediction, representation and emulation of interactive behavior 

**Application**: prediction, decision-making and behavior planning for autonomous vehicles, comprehension and modeling of interactive, social behavior, (scene/motion) representation learning and construction, imitation and generation of human (driving) behavior.

#### 1.1 Inverse optimal control (inverse reinforcement learning, IRL) and game theory

- Social factors such as courtesy (*[IROS18](https://arxiv.org/abs/1808.02633)*) and irrationality (*[ITSC19](https://arxiv.org/abs/1907.08707)*) for interactive prediction and planning with IRL.
- Interactive, probabilistic prediction with hierarchical IRL: *[ITSC18](https://arxiv.org/abs/1809.02926)*, *[ITSC19](https://arxiv.org/abs/1907.10170)*
- Learning cost for planning by IRL: *[IV19](https://arxiv.org/abs/1905.00988)*, [*TechXplore*](https://techxplore.com/news/2019-05-social-perception-scheme-behavior-autonomous.html), *ICRA20*.
- Game theory: papers to appear.

#### 1.2 Decision and planning under uncertainty with interaction

- Integrated decision/planning with interaction and negotiation: *[ITSC16](https://ieeexplore.ieee.org/abstract/document/7795595/)*, *[ACC16](https://www.researchgate.net/profile/Changliu_Liu/publication/305107862_Enabling_Safe_Freeway_Driving_for_Automated_Vehicles/links/5a7137810f7e9ba2e1cb1d90/Enabling-Safe-Freeway-Driving-for-Automated-Vehicles.pdf)*, [*SAE17*](https://www.sae.org/publications/technical-papers/content/2017-01-1406/), *[IV18-1](http://oss-cn-qingdao.aliyuncs.com/ccm-test/47d772fc485632f5b0e53977ffe59a0c.pdf)*, *[IV18-2](https://ieeexplore.ieee.org/abstract/document/8500702/)*, *[ACC19](https://arxiv.org/abs/1809.09735)*.
- Safety and feasibility in imitation learning: *[IECON17](https://ieeexplore.ieee.org/abstract/document/8216790/)*, *[DSCC18](https://arxiv.org/abs/1707.02515)*, *[IROS19](https://arxiv.org/abs/1903.00640)*.
- Reinforcement learning: *[IROS19](https://arxiv.org/abs/1904.06025)* *(**Best Paper Finalist**)*, *[IV18](https://www.researchgate.net/profile/Jianyu_Chen22/publication/328454880_Deep_Hierarchical_Reinforcement_Learning_for_Autonomous_Driving_with_Distinct_Behaviors/links/5be340a0299bf1124fc2dc59/Deep-Hierarchical-Reinforcement-Learning-for-Autonomous-Driving-with-Distinct-Behaviors.pdf)*, [*IV19*](https://ieeexplore.ieee.org/abstract/document/8813861), *[ITSC19](https://arxiv.org/abs/1904.09503)*, *[arxiv](https://arxiv.org/abs/2001.08726)*.

#### 1.3 Interactive prediction with dynamics, semantic representation and reasoning

- Semantic representation and prediction: *[IV18](https://arxiv.org/abs/1804.03629)* *(**Best Student Paper**)*, and papers to appear.
- Incorporating vehicle kinematics into deep generative models: *[IV19](https://ieeexplore.ieee.org/abstract/document/8813783)*.
- Probabilistic graphical model (*[ITSC18](https://arxiv.org/abs/1809.02927)*, *[ITSC19](https://ieeexplore.ieee.org/abstract/document/8917031)*)  and deep generative models (*[IV19](https://arxiv.org/abs/1905.00587)*, *[ICRA19-1](https://arxiv.org/abs/1904.02390)*, *[ICRA19-2](https://ieeexplore.ieee.org/abstract/document/8794130)*, *[IROS19](https://arxiv.org/abs/1905.01631)*)
- Conditional variational auto-encoder (*[ITSC18](https://arxiv.org/abs/1810.12506)*) and its interpretability (*[IV19](https://arxiv.org/abs/1903.09381)*, [*TechXplore*](https://techxplore.com/news/2019-04-sequential-motions-interacting-agents.html)), as well as the combination with IRL (*[ITSC19](https://arxiv.org/abs/1907.10170)*).
- Graph reasoning: *[arxiv-1](https://arxiv.org/pdf/2002.06241.pdf)*,  [*arxiv-2*](https://arxiv.org/abs/2003.13924), and papers to appear.
- Heterogeneous road users (pedestrian-vehicle interaction): *[ITSC19](https://ieeexplore.ieee.org/abstract/document/8917031)*, [*arxiv*](https://arxiv.org/abs/2003.13924).

#### 1.4 Scene/motion representation learning and construction

- Comprehensive scene and motion representation construction: *[IV17](https://ieeexplore.ieee.org/abstract/document/7995789/)*, and papers to appear.
- Representation learning: [*arxiv*](http://arxiv.org/abs/2003.12464), and papers to appear.



### 2. Data and perception for humans, vehicles and cities

**Application**: dataset construction for human (driving) behavior and mapping/localization, detection/tracking/mapping with onboard sensors, traffic cameras/drones, connectivity, as well as occlusion inference via behavior of others.

#### 2.1 INTERACTION Dataset: highly interactive driving behavior with semantic map

- Dataset *[website](https://interaction-dataset.com/)*, prediction challenge [*website*](http://challenge.interaction-dataset.com/prediction-challenge/intro), dataset papers (*[arxiv](https://arxiv.org/abs/1910.03088)*, *[IROS19](https://ieeexplore.ieee.org/abstract/document/8967724)*).

#### 2.2 UrbanLoco Dataset: localization and mapping in dense urban scenes

- Dataset *[website](https://advdataset2019.wixsite.com/urbanloco)*, dataset paper (*[ICRA20](https://arxiv.org/abs/1912.09513)*), [*blog*](https://medium.com/@ourxxbluesky/urbanloco-a-new-challenge-for-urban-mapping-and-localization-200742ea7629).

#### 2.3 3D detection/segmentation/reconstruction with LiDARs and cameras

- 3D segmentation and detection (with LiDAR-camera fusion): *arxiv20*, [*arxiv*](https://arxiv.org/abs/1910.04853), *[IV19](https://arxiv.org/abs/1811.03818)*, *[IV18](https://arxiv.org/abs/1711.06703)*.
- 3D point cloud reconstruction and registration: *[IROS19](https://ieeexplore.ieee.org/abstract/document/8967589)*, [*IFAC20*](https://arxiv.org/abs/1912.05016).
- Detection from bird's eye view: *[arxiv](https://arxiv.org/abs/1912.09632)*.

#### 2.4 Occluded object tracking, social perception and cooperative perception

- [*Trans-ITS*](https://arxiv.org/abs/1908.09031), *[IV18](https://arxiv.org/abs/1809.10237)*, *[IV19](https://arxiv.org/abs/1905.00988)*, [*TechXplore*](https://techxplore.com/news/2019-05-social-perception-scheme-behavior-autonomous.html).

  

### 3. Validation and simulation for autonomy and environments

**Application**: test and evaluation of prediction/planning/perception/localization modules by reconstructing the real world and utilizing high-quality data.

#### 3.1 Prediction benchmark and challenge

- Fatality-aware evaluation: *[ITSC18](https://arxiv.org/abs/1809.03478)*, *[IV18](https://hal-mines-paristech.archives-ouvertes.fr/hal-01981612/document)*.
- INTERPRET Challenge: [*website*](http://challenge.interaction-dataset.com).

#### 3.2 Uncertainty estimation and evaluation for perception and localization

- Uncertainty-aware evaluation for 3D detection: *[arxiv](https://arxiv.org/abs/2003.03644)*.
- Uncertainty estimation in LiDAR-base localization: *[IET EL Letter](https://digital-library.theiet.org/content/journals/10.1049/el.2018.8075)*.

#### 3.3 Testing prediction/decision/planning in simulation

- papers to appear



### 4. Planning, dynamics and control for autonomous systems

**Application**: Trajectory planning, dynamics modeling and controller design for passenger/delivery/racing vehicles (with connectivity).

#### 4.1 Trajectory planning

- Constrained iterative LQR and optimization: *[Trans-IV](https://ieeexplore.ieee.org/abstract/document/8671755)*, *[ITSC17](https://www.researchgate.net/profile/Jianyu_Chen22/publication/323789278_Constrained_iterative_LQR_for_on-road_autonomous_driving_motion_planning/links/5be33fd3a6fdcc3a8dc64b57/Constrained-iterative-LQR-for-on-road-autonomous-driving-motion-planning.pdf)*, *[ACC18](https://ieeexplore.ieee.org/abstract/document/8431104)*, *[IV17](https://www.researchgate.net/profile/Changliu_Liu/publication/318800685_Speed_profile_planning_in_dynamic_environments_via_temporal_optimization/links/599b6ec8a6fdcc500349c698/Speed-profile-planning-in-dynamic-environments-via-temporal-optimization.pdf)*.
- Sample-based and graph search: *IFAC20*, *[IV17-1](https://ieeexplore.ieee.org/abstract/document/7995789/),* *[IV17-2](http://www.cs.cmu.edu/~cliu6/files/iv17-1.pdf)*.

#### 4.2 Policy transfer and robust control

- *[Trans-ITS](https://ieeexplore.ieee.org/document/8924943)*, *[ITSC18](https://arxiv.org/abs/1812.03216)* *(**Best Student Paper**)*.

#### 4.3 Vehicle dynamics, state estimation and control

- System identification: *IV20*. 
- Estimation and control with connectivity: *[Sensors](https://www.mdpi.com/1424-8220/19/13/2983)*.
- Selective vehicle dynamics and control research in MSC Lab (in collaboration with California PATH) over a decade ago: 
  - Heavy-duty vehicle (truck with trailer) control: [*PATH-report*](https://www.researchgate.net/publication/46439115_Lateral_Control_of_Heavy_Duty_Vehicles_for_Automated_Highway_System_Experimental_Study_on_a_Tractor_Semi-trailer).
  - Automated highway systems: [*Trans-VT*](https://ieeexplore.ieee.org/abstract/document/69979), [*CSM*](https://ieeexplore.ieee.org/abstract/document/334412).
  - Adaptive control: [*Trans-IE*](https://ieeexplore.ieee.org/document/1174058), [*ACC90*](https://ieeexplore.ieee.org/document/4791050).
  - Preview control: [*JDSMC*](https://asmedigitalcollection.asme.org/dynamicsystems/article/115/4/679/417103/Preview-Control-for-Vehicle-Lateral-Guidance-in), [*ACC90*](https://ieeexplore.ieee.org/document/4790840).
  - Adaptive cruise control: [*IJAT*](https://link.springer.com/article/10.1007/s12239-012-0007-6), [*IFAC*](https://www.sciencedirect.com/science/article/pii/S1474667016318390).
  - Combined lateral and longitudinal control: [*SAE-IJPC*](https://saemobilus.sae.org/content/2015-01-0321), [*JDSMC*](https://asmedigitalcollection.asme.org/dynamicsystems/article/123/3/535/460331/Coordinated-Longitudinal-and-Lateral-Motion).
  - Fault tolerant control: [*Trans-Mech*](https://ieeexplore.ieee.org/abstract/document/1395861), [*IFAC*](https://www.sciencedirect.com/science/article/pii/S1474667017339198).





## Contact

Please contact Dr. Wei Zhan (wzhan@berkeley.edu) and Professor Masayoshi Tomizuka (tomizuka@berkeley.edu) for more information if you are interested in the topics above by

- working with us (join/visit the group or collaborate) from academia, or
- research collaboration from industry.