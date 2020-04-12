---
layout: page-wide
title: Autonomous Driving Group
permalink: /research/autonomous-vehicle.html
---

### Contents:

* [Introduction](#id1)
* [Research Topics](#id2)
* [Activities](#id3)
* [Contact](#id4)



## <a name="id1"></a>Introduction

The core focus of our research is to understand the interactive human (driving) behavior and the scene with proper representations, and to predict and emulate the behavior to enable safe and high-quality autonomy for various mobility. Our viewpoint is to exploit the synergies of model-based planning/control methods and state-of-the-art machine learning techniques to combine our prior and what we can learn from data. In order to sufficiently support the focus, our research scope also expands to the fundamental aspects such as validation/evaluation and dataset construction. We also dive into perception from different perspectives and control for various platforms, and incorporate our behavior-related research insights into these aspects.

<table style="position:relative;">
<tr>
<td>
<img style="width: 100%;" src="{{ site.baseurl }}/assets/images/research/autonomous/facility_data_collection_vehicle.jpg">
</td>
<td>
<img style="width: 100%;" src="{{ site.baseurl }}/assets/images/research/autonomous/facility_simulator.jpg">
</td>
<td>
<img style="width: 100%;" src="{{ site.baseurl }}/assets/images/research/autonomous/facility_autonomous_vehicles.jpg">
</td>
</tr>  
<tr>
<td>
<b>Data-collection vehicle</b>: with a high-end navigation system, and a LiDAR calibrated and synchronized with 6 cameras.
</td>
<td>
<b>Data collection and tests in simulation</b>: 2 sets of driving simulator interfaces composed with parts from real vehicles.
</td>
<td>
<b>Autonomous vehicles</b>: Our algorithms were tested on autonomous vehicles in test fields supported by our sponsors.
</td>
</tr>  
</table>


The group lead is Dr. [Wei Zhan](https://scholar.google.com/citations?user=xVN3UxYAAAAJ&hl=en#). The research activities are conducted by 2 Postdocs (Dr. [Wei Zhan](https://scholar.google.com/citations?user=xVN3UxYAAAAJ&hl=en#) and Dr. [Liting Sun](https://scholar.google.com/citations?user=BitIg-YAAAAJ&hl=en)) and 13 Ph.D. students with over 10 visiting researchers. Two datasets ([INTERACTION](https://interaction-dataset.com/) and [UrbanLoco](https://advdataset2019.wixsite.com/urbanloco)) were published. Several recent publications on autonomous driving by laboratory members received Best Student Paper or Best Paper Finalist in flagship conferences on robotics and intelligent vehicle/transportation, such as *IROS*, *ITSC* and *IV*.



## <a name="id2"></a>Research Topics

### 1. Prediction, representation and emulation of interactive behavior 

**Application**: prediction, decision-making and behavior planning for autonomous vehicles, comprehension and modeling of interactive, social behavior, (scene/motion) representation learning and construction, imitation and generation of human (driving) behavior.

#### 1.1 Inverse optimal control (inverse reinforcement learning, IRL) and game theory

<table style="position:relative;">
<tr>
<td>
<div markdown="1">
- Social factors such as courtesy (*[IROS18](https://arxiv.org/abs/1808.02633)*) and irrationality (*[ITSC19](https://arxiv.org/abs/1907.08707)*) for interactive prediction and planning with IRL.
- Interactive, probabilistic prediction with hierarchical IRL: *[ITSC18](https://arxiv.org/abs/1809.02926)*, *[ITSC19](https://arxiv.org/abs/1907.10170)*
- Learning cost for planning by IRL: *[IV19](https://arxiv.org/abs/1905.00988)*, [*TechXplore*](https://techxplore.com/news/2019-05-social-perception-scheme-behavior-autonomous.html), *ICRA20*.
- Game theory: papers to appear.
</div>
</td>
<td>
<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/DQNjaNGoX2g" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
</td>
</tr>
</table>
#### 1.2 Decision and planning under uncertainty with interaction

<table style="position:relative;">
<tr>
<td>
<div markdown="1">

- Integrated decision/planning with interaction and negotiation: *[ITSC16](https://ieeexplore.ieee.org/abstract/document/7795595/)*, *[ACC16](https://www.researchgate.net/profile/Changliu_Liu/publication/305107862_Enabling_Safe_Freeway_Driving_for_Automated_Vehicles/links/5a7137810f7e9ba2e1cb1d90/Enabling-Safe-Freeway-Driving-for-Automated-Vehicles.pdf)*, [*SAE17*](https://www.sae.org/publications/technical-papers/content/2017-01-1406/), *[IV18-1](http://oss-cn-qingdao.aliyuncs.com/ccm-test/47d772fc485632f5b0e53977ffe59a0c.pdf)*, *[IV18-2](https://ieeexplore.ieee.org/abstract/document/8500702/)*, *[ACC19](https://arxiv.org/abs/1809.09735)*.
- Safety and feasibility in imitation learning: *[IECON17](https://ieeexplore.ieee.org/abstract/document/8216790/)*, *[DSCC18](https://arxiv.org/abs/1707.02515)*, *[IROS19](https://arxiv.org/abs/1903.00640)*.
- Reinforcement learning: *[IROS19](https://arxiv.org/abs/1904.06025)* *(**Best Paper Finalist**)*, *[IV18](https://www.researchgate.net/profile/Jianyu_Chen22/publication/328454880_Deep_Hierarchical_Reinforcement_Learning_for_Autonomous_Driving_with_Distinct_Behaviors/links/5be340a0299bf1124fc2dc59/Deep-Hierarchical-Reinforcement-Learning-for-Autonomous-Driving-with-Distinct-Behaviors.pdf)*, [*IV19*](https://ieeexplore.ieee.org/abstract/document/8813861), *[ITSC19](https://arxiv.org/abs/1904.09503)*, *[arxiv](https://arxiv.org/abs/2001.08726)*.
</div>
</td>
<td>
<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="http://www.youtube.com/embed/pvHaYfN7Ciw" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
</td>
</tr>
</table>

#### 1.3 Interactive prediction with dynamics, semantic representation and reasoning

<table style="position:relative;">
<tr>
<td>
<div markdown="1">

- Semantic representation and prediction: *[IV18](https://arxiv.org/abs/1804.03629)* *(**Best Student Paper**)*, [*arxiv*](https://arxiv.org/abs/2004.03053).
- Incorporating vehicle kinematics into deep generative models: *[IV19](https://ieeexplore.ieee.org/abstract/document/8813783)*.
- Probabilistic graphical model (*[ITSC18](https://arxiv.org/abs/1809.02927)*, *[ITSC19](https://ieeexplore.ieee.org/abstract/document/8917031)*)  and deep generative models (*[IV19](https://arxiv.org/abs/1905.00587)*, *[ICRA19-1](https://arxiv.org/abs/1904.02390)*, *[ICRA19-2](https://ieeexplore.ieee.org/abstract/document/8794130)*, *[IROS19](https://arxiv.org/abs/1905.01631)*)
- Conditional variational auto-encoder (*[ITSC18](https://arxiv.org/abs/1810.12506)*) and its interpretability (*[IV19](https://arxiv.org/abs/1903.09381)*, [*TechXplore*](https://techxplore.com/news/2019-04-sequential-motions-interacting-agents.html)), as well as the combination with IRL (*[ITSC19](https://arxiv.org/abs/1907.10170)*).
- Graph reasoning: [*arxiv-1*](https://arxiv.org/abs/2004.03053), *[arxiv-2](https://arxiv.org/pdf/2002.06241.pdf)*,  [*arxiv-3*](https://arxiv.org/abs/2003.13924).

</div>
</td>
<td>
<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/6A3Hl-mRhbI" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
</td>
</tr>
</table>

#### 1.4 Scene/motion representation learning and construction

<table style="position:relative;">
<tr>
<td>
<div markdown="1">
- Comprehensive scene and motion representation construction: *[IV17](https://ieeexplore.ieee.org/abstract/document/7995789/)*, [*arxiv*](https://arxiv.org/abs/2004.03053).
- Representation learning: [*arxiv*](http://arxiv.org/abs/2003.12464), and papers to appear.
</div>
</td>
</tr>
</table>


### 2. Data and perception for humans, vehicles and cities

**Application**: dataset construction for human (driving) behavior and mapping/localization, detection/tracking/mapping with onboard sensors, traffic cameras/drones, connectivity, as well as occlusion inference via behavior of others.

#### 2.1 INTERACTION Dataset: highly interactive driving behavior with semantic map
<table style="position:relative;">
<tr>
<td>
<div markdown="1">
- Dataset *[website](https://interaction-dataset.com/)*, prediction challenge [*website*](http://challenge.interaction-dataset.com/prediction-challenge/intro), dataset papers (*[arxiv](https://arxiv.org/abs/1910.03088)*, *[IROS19](https://ieeexplore.ieee.org/abstract/document/8967724)*).
</div>
</td>
</tr>
</table>
#### 2.2 UrbanLoco Dataset: localization and mapping in dense urban scenes
<table style="position:relative;">
<tr>
<td>
<div markdown="1">
- Dataset *[website](https://advdataset2019.wixsite.com/urbanloco)*, dataset paper (*[ICRA20](https://arxiv.org/abs/1912.09513)*), [*blog*](https://medium.com/@ourxxbluesky/urbanloco-a-new-challenge-for-urban-mapping-and-localization-200742ea7629).
</div>
</td>
</tr>
</table>
#### 2.3 3D detection/segmentation/reconstruction with LiDARs and cameras
<table style="position:relative;">
<tr>
<td>
<div markdown="1">
- 3D segmentation and detection (with LiDAR-camera fusion): [*arxiv-1*](https://arxiv.org/abs/2004.01803), [*arxiv-2*](https://arxiv.org/abs/1910.04853), *[IV19](https://arxiv.org/abs/1811.03818)*, *[IV18](https://arxiv.org/abs/1711.06703)*.
- 3D point cloud reconstruction and registration: *[IROS19](https://ieeexplore.ieee.org/abstract/document/8967589)*, [*IFAC20*](https://arxiv.org/abs/1912.05016).
- Detection from bird's eye view: *[arxiv](https://arxiv.org/abs/1912.09632)*.
</div>
</td>
</tr>
</table>
#### 2.4 Occluded object tracking, social perception and cooperative perception
<table style="position:relative;">
<tr>
<td>
<div markdown="1">
- [*Trans-ITS*](https://arxiv.org/abs/1908.09031), *[IV18](https://arxiv.org/abs/1809.10237)*, *[IV19](https://arxiv.org/abs/1905.00988)*, [*TechXplore*](https://techxplore.com/news/2019-05-social-perception-scheme-behavior-autonomous.html).
</div>
</td>
</tr>
</table>
  

### 3. Validation and simulation for autonomy and environments

**Application**: test and evaluation of prediction/planning/perception/localization modules by reconstructing the real world and utilizing high-quality data.

#### 3.1 Prediction benchmark and challenge
<table style="position:relative;">
<tr>
<td>
<div markdown="1">
- Fatality-aware evaluation: *[ITSC18](https://arxiv.org/abs/1809.03478)*, *[IV18](https://hal-mines-paristech.archives-ouvertes.fr/hal-01981612/document)*.
- INTERPRET Challenge: [*website*](http://challenge.interaction-dataset.com).
</div>
</td>
</tr>
</table>
#### 3.2 Uncertainty estimation and evaluation for perception and localization
<table style="position:relative;">
<tr>
<td>
<div markdown="1">
- Uncertainty-aware evaluation for 3D detection: *[arxiv](https://arxiv.org/abs/2003.03644)*.
- Uncertainty estimation in LiDAR-base localization: *[IET EL Letter](https://digital-library.theiet.org/content/journals/10.1049/el.2018.8075)*.
</div>
</td>
</tr>
</table>
#### 3.3 Testing prediction/decision/planning in simulation
<table style="position:relative;">
<tr>
<td>
<div markdown="1">
- papers to appear
</div>
</td>
</tr>
</table>

### 4. Planning, dynamics and control for autonomous systems

**Application**: Trajectory planning, dynamics modeling and controller design for passenger/delivery/racing vehicles (with connectivity).

#### 4.1 Trajectory planning
<table style="position:relative;">
<tr>
<td>
<div markdown="1">
- Constrained iterative LQR and optimization: *[Trans-IV](https://ieeexplore.ieee.org/abstract/document/8671755)*, *[ITSC17](https://www.researchgate.net/profile/Jianyu_Chen22/publication/323789278_Constrained_iterative_LQR_for_on-road_autonomous_driving_motion_planning/links/5be33fd3a6fdcc3a8dc64b57/Constrained-iterative-LQR-for-on-road-autonomous-driving-motion-planning.pdf)*, *[ACC18](https://ieeexplore.ieee.org/abstract/document/8431104)*, *[IV17](https://www.researchgate.net/profile/Changliu_Liu/publication/318800685_Speed_profile_planning_in_dynamic_environments_via_temporal_optimization/links/599b6ec8a6fdcc500349c698/Speed-profile-planning-in-dynamic-environments-via-temporal-optimization.pdf)*.
- Sample-based and graph search: *IFAC20*, *[IV17-1](https://ieeexplore.ieee.org/abstract/document/7995789/),* *[IV17-2](http://www.cs.cmu.edu/~cliu6/files/iv17-1.pdf)*.
</div>
</td>
</tr>
</table>
#### 4.2 Policy transfer and robust control
<table style="position:relative;">
<tr>
<td>
<div markdown="1">
- *[Trans-ITS](https://ieeexplore.ieee.org/document/8924943)*, *[ITSC18](https://arxiv.org/abs/1812.03216)* *(**Best Student Paper**)*.
</div>
</td>
</tr>
</table>
#### 4.3 Vehicle dynamics, state estimation and control
<table style="position:relative;">
<tr>
<td>
<div markdown="1">
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
</div>
</td>
</tr>
</table>


## <a name="id3"></a>Activities

- **[ITSC 2020](https://www.ieee-itsc2020.org) Workshop** (Rhodes, Greece, September 2020): [Probabilistic Prediction and Comprehensible Motion Planning for Automated Vehicles – Approaches and Benchmarking](https://ieee-itsc2020.org/wp-content/uploads/2020/03/Probabilistic-Prediction-and-Comprehensible-Motion-Planning-for-Automated-Vehicles-–-Approaches-and-Benchmarking.pdf), organized by Maximilian Naumann, Martin Lauer, Liting Sun, Wei Zhan, Masayoshi Tomizuka, Arnaud de La Fortelle, Christoph Stiller.
- **[RSS 2020](https://roboticsconference.org) Workshop** (virtual, June 2020): Interaction and Decision-Making in Autonomous-Driving, organized by Rowan McAllister, Liting Sun, Igor Gilitschenski, Daniela Rus.
- The results of the first round [INTERPRET Challenge](http://challenge.interaction-dataset.com/prediction-challenge/intro) will be presented in **[CVPR 2020](http://cvpr2020.thecvf.com) Workshop** (Seattle, June 2020) organized by Waymo: [Scalability in Autonomous Driving](https://sites.google.com/view/cvpr20-scalability). 
- **[IV 2020](https://2020.ieee-iv.org) Joint Workshops** (Las Vegas, postponed to October 2020): [From Benchmarking Behavior Prediction to Socially Compatible Behavior Generation in Autonomous Driving](https://sites.google.com/berkeley.edu/iv20-interaction/home), organized by Wei Zhan, Liting Sun, Maximilian Naumann. Jiachen Li and Masayoshi Tomizuka.
- **[IROS 2019](https://www.iros2019.org) Workshop** (Macao, November 2019): [Benchmark and Dataset for Probabilistic Prediction of Interactive Human Behavior](https://sites.google.com/berkeley.edu/iros2019-ws-dataset-benmark/home), organized by Wei Zhan, Liting Sun and Masayoshi Tomizuka.
- **[IV 2019](https://iv2019.org) Workshop** (Paris, June 2019): [Prediction and Decision Making for Socially Interactive Autonomous Driving](https://sites.google.com/berkeley.edu/iv19-interaction), organized by Wei Zhan, Jiachen Li, Liting Sun, Yeping Hu and Masayoshi Tomizuka.



## <a name="id4"></a>Contact

Please contact Dr. Wei Zhan (wzhan@berkeley.edu) and Professor Masayoshi Tomizuka (tomizuka@berkeley.edu) for more information if you are interested in the topics above by

- working with us (join/visit the group or collaborate) from academia, or
- research collaboration from industry.

<img width = "100%" src="{{ site.baseurl }}/assets/images/research/autonomous/headshots.jpg">


