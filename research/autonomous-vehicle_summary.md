---
layout: page-wide
title: Autonomous Driving Group
permalink: /research/autonomous-vehicle.html
---

### Contents:

* [Introduction](#intro)
* [Facilities and Datasets](#id2)
* [Activities](#activity)
* [Research Topics](#research)
* [Joining Our Group](#join)
* [Members and Contact](#id5)



## <a name="intro"></a>Introduction

Our research covers full-stack autonomous driving, including the onboard modules such as perception, prediction, planning and control, as well as key offline components such as simulation/test, and automatic construction of HD maps and data. The efforts have been greatly supported and intensively verified by the facilities including autonomous vehicles, data-collection vehicles, and driving simulators. We also constructed datasets by our own, such as [INTERACTION](https://interaction-dataset.com/) dataset for behavior/prediction and [UrbanLoco](https://advdataset2019.wixsite.com/urbanloco) dataset for localization/mapping. Our recent progress has been published in flagship conferences in the fields of robotics (*ICRA, IROS*), computer vision (*CVPR, ECCV*), machine learning and AI (*NeurIPS, AAAI*), intelligent transportation (*ITSC, IV*) and control (*ACC, IFAC*) and corresponding top-notch journals. We received several Best (Student) Paper Awards/Finalists from *IROS*, *ITSC* and *IV*.

<table style="position:relative;">
<tr>
<td>
<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/v__zuUw3GZI?playlist=v__zuUw3GZI&autoplay=1&mute=1&loop=1&playlist=8HSr8BjcufM&amp" frameborder="0" allow="autoplay; encrypted-media" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
</td>
<td>
<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/avTP-FJgmDI?playlist=avTP-FJgmDI&autoplay=1&mute=1&loop=1" frameborder="0" allow="autoplay; encrypted-media" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
</td>
<td>
<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/lJWAEMhGgkU?playlist=lJWAEMhGgkU&autoplay=1&mute=1&loop=1" frameborder="0" allow="autoplay; encrypted-media" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
</td>
</tr>  
<tr>
<td>
<b>Perception</b>: 3D/2D detection, segmentation, LiDAR-camera fusion, evaluation, tracking, inference.
</td>
<td>
<b>Mapping and localization</b>: Automatic construction of HD map, point cloud map construction and localization.
</td>
<td>
<b>Behavioral data, simulation and test</b>: Behavior dataset construction, closed-loop test, scenario/behavior generation, human-in-loop test.
</td>
</tr>  
</table>


<table style="position:relative;">
<tr>
<td>
<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/OLtPAmrfUkE?playlist=OLtPAmrfUkE&autoplay=1&mute=1&loop=1" frameborder="0" allow="autoplay" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
</td>
<td>
<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/fHcGzx1eh-Y?playlist=fHcGzx1eh-Y&autoplay=1&mute=1&loop=1" frameborder="0" allow="autoplay" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
</td>
<td>
<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/sLV49jbJOP4?playlist=sLV49jbJOP4&autoplay=1&mute=1&loop=1" frameborder="0" allow="autoplay" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
</td>
</tr>  
<tr>
<td>
<b>Prediction and behavior generation</b>: interactive prediction, representation, generalization, behavior understanding and generation.
</td>
<td>
<b>Decision and behavior planning</b>: interactive decision-making and planning under uncertainty, incorporating learning and model-based methods.
</td>
<td>
<b>Motion planning and control</b>: safe and efficient trajectory planning, autonomous racing, policy transfer, vehicle dynamics and control.
</td>
</tr>  
</table>

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
<b>Data collection and tests in simulation</b>: Two sets of driving simulator interfaces composed with parts from real vehicles.
</td>
<td>
<b>Autonomous vehicles</b>: Our algorithms were tested on autonomous vehicles in test fields supported by our sponsors.
</td>
</tr>  
</table>

## <a name="research"></a>Research Topics

### 1. Perception

Perception is a prerequisite for autonomy. 3D perception based on LiDAR (and camera) is our major focus. We are interested in incorporating temporal information for 3D perception and its synergies with downstream modules such as prediction. Computationally efficient and data-efficient 3D perception is also addressed with novel structures, self-supervision and multi-task learning. Early-stage and cascade LiDAR-camera fusion approaches are proposed for 3D detection. We also dive into fundamental problems in 3D detection by analyzing and inferring uncertainties of the data annotations, as well as evaluating and improving probabilistic 3D detection. In addition to 3D perception, new structures are proposed for 2D detection, segmentation and crowd count. We also emphasize occluded object tracking and inference via the behavior of the surrounding agents of the object.

#### 1.1 3D perception

<table style="position:relative;">
<tr>
<td>
<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/v__zuUw3GZI?playlist=v__zuUw3GZI&autoplay=1&mute=1&loop=1&playlist=8HSr8BjcufM&amp" frameborder="0" allow="autoplay; encrypted-media" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
</td>
<td>
<img style="width: 100%;" src="{{ site.baseurl }}/assets/images/research/autonomous/3Dperception_uncertainty.png">
</td>
<td>
<img style="width: 100%;" src="{{ site.baseurl }}/assets/images/research/autonomous/3Dperception_fusion.png">
</td>
</tr>  
<tr>
<td>
<div markdown="1">
- <b>3D segmentation</b> for point cloud with spatially adaptive convolution: *[ECCV20](https://arxiv.org/abs/2004.01803)*.
</div>
</td>
<td>
<div markdown="1">
- <b>Uncertainty-aware 3D detection</b>: evaluation, labeling analysis and performance improvement (*[Trans-ITS](https://arxiv.org/abs/2012.12195)*, *[IROS20](https://arxiv.org/abs/2003.03644)*, *[ITSC20](https://arxiv.org/abs/2006.12015)*).
</div>
</td>
<td>
<div markdown="1">
  - <b>LiDAR-camera fusion</b> for 3D detection: *[IV18](https://arxiv.org/abs/1711.06703)*, *[IV19](https://arxiv.org/abs/1811.03818)*, [*IV20*](https://arxiv.org/abs/1910.04853).
</div>
</td>
</tr>  
</table>

<table style="position:relative;">
<tr>
<td>
<img style="width: 100%;" src="{{ site.baseurl }}/assets/images/research/autonomous/3Dperception_multitask.png">
</td>
<td>
<img style="width: 100%;" src="{{ site.baseurl }}/assets/images/research/autonomous/3Dperception_YOGO.png">
</td>
<td>
<img style="width: 100%;" src="{{ site.baseurl }}/assets/images/research/autonomous/3Dperception_registration.png">
</td>
</tr>  
<tr>
<td>
<div markdown="1">
- <b>Multi-task learning</b> for efficient 3D detection and road understanding ([*arxiv*)](https://arxiv.org/abs/2103.04056).
</div>
</td>
<td>
<div markdown="1">
- <b>Token representation</b> for efficient point cloud processing (*[arxiv](https://arxiv.org/abs/2103.09975)*).
</div>
</td>
<td>
<div markdown="1">
- <b>Reconstruction and registration</b> for 3D point cloud: *[IROS19](https://ieeexplore.ieee.org/abstract/document/8967589)*, [*IFAC20*](https://arxiv.org/abs/1912.05016).
</div>
</td>
</tr>  
</table>

#### 1.2 2D perception

<table style="position:relative;">
<tr>
<td>
<img style="width: 100%;" src="{{ site.baseurl }}/assets/images/research/autonomous/2Dperception_AutoScale.jpg">
</td>
<td>
<img style="width: 100%;" src="{{ site.baseurl }}/assets/images/research/autonomous/2Dperception_SparceRCNN.jpg">
</td>
</tr>
<tr>
<td>
<div markdown="1">
<b>AutoScale</b> [*arxiv*](https://arxiv.org/abs/1912.09632): crowd counting and localization.
</div>
</td>
<td>
<div markdown="1">
<b>Sparse R-CNN</b> ([*CVPR21*](https://arxiv.org/abs/2011.12450)) and Visual Transformers (*[arxiv](https://arxiv.org/abs/2006.03677)*).
</div>
</td>
</tr>  
</table>


#### 1.3 Occluded object tracking and inference

- Occluded object tracking by inferring from motions of its surrounding objects: [*Trans-ITS*](https://arxiv.org/abs/1908.09031), *[IV18](https://arxiv.org/abs/1809.10237)*. 
- Social perception to infer existence of occluded objects from behavior of others: *[IV19](https://arxiv.org/abs/1905.00988)*, [*TechXplore*](https://techxplore.com/news/2019-05-social-perception-scheme-behavior-autonomous.html).
- Cooperative perception to achieve better detection and tracking of occluded object via connectivity.



### 2. Mapping and Localization

We consider two aspects in mapping/localization research, namely, localization-oriented including point cloud map construction and localization based on multi-sensor fusion, as well as semantic-oriented to understand the scene/road and construct HD maps for prediction/planning modules. Our major focus is to automatically construct semantic HD maps by reconstructing the road geometry from low-cost sensor data, and inferring the topology and semantics via road/scene understanding models and rough navigation maps. We also built the UrbanLoco dataset with full sensor suite to test the mapping and localization algorithms in dense urban scenarios such as downtown San Francisco and Hong Kong.

#### 2.1 Automatic HD map construction and scene understanding

<table style="position:relative;">
<tr>
<td>
<img style="width: 100%;" src="{{ site.baseurl }}/assets/images/research/autonomous/mapping.png">
</td>
</tr> 
</table>

- Automatic construction of semantic HD map utilizing rough navigation map: paper to appear.
- Road and scene understanding.

#### 2.2 Localization and point cloud map construction

<table style="position:relative;">
<tr>
<td>
<img style="width: 100%;" src="{{ site.baseurl }}/assets/images/research/autonomous/localization_urbanloco.png">
</td>
</tr> 
</table>

- Mapping and localization dataset in highly urbanized scenes -- UrbanLoco dataset: [website](https://advdataset2019.wixsite.com/urbanloco), dataset paper (*[ICRA20](https://arxiv.org/abs/1912.09513)*), [blog](https://medium.com/@ourxxbluesky/urbanloco-a-new-challenge-for-urban-mapping-and-localization-200742ea7629), [video](https://youtu.be/3axr7ICggRw).

<table style="position:relative;">
<tr>
<td>
<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/CDp6mocT6C4?playlist=CDp6mocT6C4&autoplay=1&mute=1&loop=1" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
</td>
<td>
<img style="width: 100%;" src="{{ site.baseurl }}/assets/images/research/autonomous/localization_EP.png">
</td>
<td>
<img style="width: 100%;" src="{{ site.baseurl }}/assets/images/research/autonomous/localization_downtown.png">
</td>
</tr> 
</table>

- Uncertainty estimation in LiDAR-base localization: *[IET Electronics Letters](https://digital-library.theiet.org/content/journals/10.1049/el.2018.8075)*.
- City-scale mapping and localization with object removal.



### 3. Behavior Data, Simulation and Evaluation 

One of the most challenging tasks in autonomous driving is to understand, predict and react to interactive behavior of surrounding agents in complex scenarios. To enable and support the research in these fields, there are several fundamental aspects to address, including behavior data in highly interactive scenarios with HD maps, as well as structure, metrics, and generation of reactive behavior and scenarios in simulation and test of the prediction/planning algorithms. We construct the INTERACTION dataset, which contains densely interactive/critical behavior from international locations along with the semantic HD maps, which has been widely used and serves as basis for our behavior-related research from simulation, generation, extraction, to prediction, decision and planning. We also proposed closed-loop structure and metrics for prediction with competitions organized. Research efforts are also devoted to the generation of critical and natural behavior, as well as scenarios in simulation.

#### 3.1 Behavior dataset construction

<table style="position:relative;">
<tr>
<td>
<div markdown="1">
- Densely interactive beahvior and critical situations in complex scenarios: negotiations, inexplicit right-of-way, irrational behavior, near-collision situations, violation of traffic rules.
- Highly accurate trajectories and complete information of surroundings.
- HD maps with full semantics required by prediction and planning algorithms.
- International locations (US, Germany, China) with diversified scenarios (roundabouts, signalized/unsignalized intersections, highway/urban merging and lane change).
- Dataset *[website](https://interaction-dataset.com/)*, and papers (*[arxiv](https://arxiv.org/abs/1910.03088)*, *[IROS19](https://ieeexplore.ieee.org/abstract/document/8967724)*).
- Prediction challenge [*website*](http://challenge.interaction-dataset.com/prediction-challenge/intro)
</div>
</td>
<td>
<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/6n6FkYwL08g" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
</td>
</tr>
</table>

#### 3.2 Closed-loop evaluation of prediction

- Fatality-aware evaluation of prediction: *[ITSC18](https://arxiv.org/abs/1809.03478)*, *[IV18](https://hal-mines-paristech.archives-ouvertes.fr/hal-01981612/document)*.
- INTERPRET Challenge as a [*NeurIPS 2020 competition*](http://challenge.interaction-dataset.com).
- Closed-loop evaluation of prediction: paper to appear.

#### 3.3 Scenario/behavior generation in simulation and test

- Critical and natural behavior generation of agents in simulation: *[arxiv](https://arxiv.org/abs/2103.00906)*.
- Scenario generation with genetic algorithms: paper to appear.
- Human-in-loop simulation and test.



### 4. Behavior Generation, Analysis, Extraction and Representation

To enable accurate prediction of interactive behavior, or human-like, safe and high-quality reactive decision/planning, or generate natural behavior in simulation, we need to understand and analyze large amount of interactive behavior data, and express, learn and generate human-like reactive behavior from the perspective of fundamental theories to model human behavior and interactions. We bring in game theory as well as other theories in economy/psychology such as cumulative prospective theory, to express and model interactive behavior with irrationalities regarding utilities and risks. These theories are incorporated with machine learning and control, such as inverse reinforcement learning, to make the reward and other key parameters learnable. We also propose models based on unsupervised/multi-task learning for extracting interactive behavior and patterns from human driving data.

#### 4.1 Event extraction and representation learning 

- Interactive behavior extraction and unsupervised learning of interaction patterns: *[RA-Letters/ICRA21](https://ieeexplore.ieee.org/abstract/document/9363585/)*.

#### 4.2 Human-like interactive behavior generation and analysis

- Courtesy- and confidence-aware inference and generation for socially-compatible and human-like driving behavior: *[RA-Letters/ICRA21](https://ieeexplore.ieee.org/abstract/document/9361150)*.
- Human-like behavior generation based on game theoretic strategies: *[IROS20](https://ras.papercept.net/proceedings/IROS20/2174.pdf)*.
- Expressing irrationality of human behaviors via a risk-sensitive inverse reinforcement learning: *[ITSC19](https://arxiv.org/abs/1907.08707)*.
- Bounded risk-sensitive Markov games considering irrationality for both policy design and reward learning: *[AAAI21](https://www.aaai.org/AAAI21Papers/AAAI-10238.TianR.pdf)*.
- Multi-agent inverse reinforcement learning by inferring latent intelligence levels of game: *[arxiv](https://arxiv.org/abs/2103.04289)*.

#### 4.3 Reward learning

- Efficient sampling-based maximum entropy inverse reinforcement learning: *[RA-Letters/IROS20](https://arxiv.org/abs/2006.13704)*.
- Probabilistic reward learning and online inference for diverse driving behavior: *[IROS20](https://arxiv.org/abs/2008.08812)*.
- Learning generic and suitable cost functions for driving: *[ICRA20](https://ras.papercept.net/proceedings/ICRA20/0320.pdf).*



### 5. Behavior Prediction

Interactive behavior prediction is a prerequisite for the decision and planning in highly interactive scenarios, which is very challenging. We proposed various models based on graph neural network, conditional variational auto-encoder and other deep generative models to enable interactive prediction for multiple, heterogeneous agents (vehicle, pedestrians, etc.). We also proposed planning-based prediction methods based on inverse reinforcement learning, which inherently predicts the reaction of others given future plans of the ego vehicle. Furthermore, we dive into the generic representation of the semantics for all static and dynamic elements in a variety of driving scenarios, and encode such representation to a semantic graph so that zero-shot scenario-transferable prediction is enabled.

#### 5.1 Representation and transferability for prediction

- Semantic representation and prediction: *[IV18](https://arxiv.org/abs/1804.03629)* *(**Best Student Paper**)*, 
- Generic scene/map/motion representation encoded to semantic graph enabling zero-shot scenario-transferable prediction: [*arxiv*](https://arxiv.org/abs/2004.03053).

#### 5.2 Interactive prediction

- Prediction based on graph neural network: *[NeurIPS20](https://arxiv.org/abs/2003.13924)*, [*arxiv*](https://arxiv.org/abs/2003.13924).
- Conditional variational auto-encoder (*[ITSC18](https://arxiv.org/abs/1810.12506)*) and its interpretability (*[IV19](https://arxiv.org/abs/1903.09381)*, [*TechXplore*](https://techxplore.com/news/2019-04-sequential-motions-interacting-agents.html)).
- Deep generative models (*[IV19](https://arxiv.org/abs/1905.00587)*, *[ICRA19-1](https://arxiv.org/abs/1904.02390)*, *[ICRA19-2](https://ieeexplore.ieee.org/abstract/document/8794130)*, *[IROS19](https://arxiv.org/abs/1905.01631)*) incorporating vehicle kinematics (*[IV19](https://ieeexplore.ieee.org/abstract/document/8813783)*).
- Probabilistic graphical model based on hidden Markov model (*[ITSC18](https://arxiv.org/abs/1809.02927)*) and dynamic Bayesian network (*[ITSC19](https://ieeexplore.ieee.org/abstract/document/8917031)*).

#### 5.3 Planning-based reaction prediction

- Hierarchical inverse reinforcement learning predicting reactions given ego plan: *[ITSC18](https://arxiv.org/abs/1809.02926)*.
- A better prediction model by online combination of deep learning with inverse reinforcement learning: *[ITSC19](https://arxiv.org/abs/1907.10170)*.



### 6. Decision and Behavioral Planning

Autonomous vehicles need to make decisions and plan behavior interactively, which are safe and human-like with desirable driving quality. One of our focuses is to design the structure of interactive decision and planning with probabilistic prediction based on POMDP, reachability and optimization/sample-based planners. Learning-based decision under uncertainty methods are proposed with hierarchical or modularized structure. We also address the combination of machine learning (imitation/reinforcement learning) and model-based methods (model predictive control/optimal control) to utilize the advantages of both. 

#### 6.1 Interactive decision and planning with probabilistic prediction

- Integrated decision and planning to achieve non-conservatively defensive strategy: *[ITSC16](https://ieeexplore.ieee.org/abstract/document/7795595/)*, *[IV18](http://oss-cn-qingdao.aliyuncs.com/ccm-test/47d772fc485632f5b0e53977ffe59a0c.pdf)*. 
- Prediction-based reachability for safe decision and planning: *[ICRA21](https://arxiv.org/abs/2011.12406)*.
- Interactive decision and planning under uncertainty with POMDP (*[DSCC20](https://asmedigitalcollection.asme.org/DSCC/proceedings-abstract/DSCC2020/1096558)*) and optimization-based negotiation (*[IV18](https://ieeexplore.ieee.org/abstract/document/8500702/)*, *[ACC19](https://arxiv.org/abs/1809.09735)*).
- Robustly safe automated driving system: *[ACC16](https://www.researchgate.net/profile/Changliu_Liu/publication/305107862_Enabling_Safe_Freeway_Driving_for_Automated_Vehicles/links/5a7137810f7e9ba2e1cb1d90/Enabling-Safe-Freeway-Driving-for-Automated-Vehicles.pdf)*, [*SAE17*](https://www.sae.org/publications/technical-papers/content/2017-01-1406/).

#### 6.2 Safe and human-like decision and planning incorporating learning and model-based methods

- Safe and feasible imitation learning: *[IECON17](https://ieeexplore.ieee.org/abstract/document/8216790/)*, *[DSCC18](https://arxiv.org/abs/1707.02515)*, *[IROS19](https://arxiv.org/abs/1903.00640)*.
- Hierarchical framework with safe planning and reinforcement learning decision-making: *[ICRA21](https://arxiv.org/abs/2101.06778)*.
- Imitating social behavior with courtesy via inverse optimal control: *[IROS18](https://arxiv.org/abs/1808.02633)*.

#### 6.3 Learning-based decision under uncertainty

- Hierarchical reinforcement learning (*[IV18](https://www.researchgate.net/profile/Jianyu_Chen22/publication/328454880_Deep_Hierarchical_Reinforcement_Learning_for_Autonomous_Driving_with_Distinct_Behaviors/links/5be340a0299bf1124fc2dc59/Deep-Hierarchical-Reinforcement-Learning-for-Autonomous-Driving-with-Distinct-Behaviors.pdf)*) and modularized network for driving policy (*[IV19](https://ieeexplore.ieee.org/abstract/document/8813861)*).
- Deep reinforcement learning: *[IROS19](https://arxiv.org/abs/1904.06025)* *(**Best Paper Finalist**)*, *[ITSC19](https://arxiv.org/abs/1904.09503)*, *[Trans-ITS](https://arxiv.org/abs/2001.08726)*.



### 7. Motion Planning and Control

Safe and high-quality trajectory planning is crucial for autonomy. We proposed various approaches based on optimal control, optimization, sampling and graph search to enable such capabilities. Generic scene representation with novel partition of the spatiotemporal domain for planning is also proposed to cover a wide variety of scenarios. In addition to the conventional vehicle dynamics and control research, we also combine  it with learning-based methods to enable policy transfer over different vehicle platforms and environments. Moreover, autonomous racing becomes a major application for our planning and control related research due to the sophisticated vehicle dynamics and complex interaction, and we build autonomous racers beating human expert drivers. Autonomous delivery is another focus of our dynamics and control research with significantly varying environments.

#### 7.1 Trajectory planning

<table style="position:relative;">
<tr>
<td>
<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/-VA_6LmLi4U?playlist=-VA_6LmLi4U&autoplay=1&mute=1&loop=1" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
</td>
<td>
<img style="width: 100%;" src="{{ site.baseurl }}/assets/images/research/autonomous/planning_generic.png">
</td>
<td>
<img style="width: 100%;" src="{{ site.baseurl }}/assets/images/research/autonomous/planning_sample.png">
</td>
</tr>   
</table>

- Generic scene representation and spatiotemporal domain patition: [*IV17*](https://ieeexplore.ieee.org/abstract/document/7995789/).
- Optimal-control-based method -- constrained iterative LQR: *[Trans-IV](https://ieeexplore.ieee.org/abstract/document/8671755)*, *[ITSC17](https://www.researchgate.net/profile/Jianyu_Chen22/publication/323789278_Constrained_iterative_LQR_for_on-road_autonomous_driving_motion_planning/links/5be33fd3a6fdcc3a8dc64b57/Constrained-iterative-LQR-for-on-road-autonomous-driving-motion-planning.pdf)*, [*DSCC20*](https://asmedigitalcollection.asme.org/DSCC/proceedings-abstract/DSCC2020/1096470).
- Temporal optimization for speed planning (*[IV17](https://www.researchgate.net/profile/Changliu_Liu/publication/318800685_Speed_profile_planning_in_dynamic_environments_via_temporal_optimization/links/599b6ec8a6fdcc500349c698/Speed-profile-planning-in-dynamic-environments-via-temporal-optimization.pdf)*) and optimization-based planning (*[ACC18](https://ieeexplore.ieee.org/abstract/document/8431104)*)
- Planning based on adaptive sampling ([*IFAC20*](https://www.sciencedirect.com/science/article/pii/S2405896320332237)) and graph search (*[IV17](http://www.cs.cmu.edu/~cliu6/files/iv17-1.pdf)*).

#### 7.2 Vehicle dynamics and control

<table style="position:relative;">
<tr>
<td>
<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/WV4hSKUA3uY?playlist=WV4hSKUA3uY&autoplay=1&mute=1&loop=1" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
</td>
<td>
<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/RvjI4cpZAAE?playlist=RvjI4cpZAAE&autoplay=1&mute=1&loop=1" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
</td>
</tr>  
<tr>
<td>
<div markdown="1">
<b>Autonomous racing</b>: Planning and control tackling sophisticated vehicle dynamics, beating human expert drivers: paper to appear.
</div>
</td>
<td>
<div markdown="1">
<b>State estimation and control (with connectivity)</b>: cooperative adaptive cruise control (CACC), remote control (*[Sensors](https://www.mdpi.com/1424-8220/19/13/2983)*), system identification (*[IV20](https://ieeexplore.ieee.org/abstract/document/9304586)*), joint estimation of state and model parameters (paper to appear).
</div>
</td>
</tr>  
</table>

<table style="position:relative;">
<tr>
<td>
<img style="width: 100%;" src="{{ site.baseurl }}/assets/images/research/autonomous/control_transfer.png">
</td>
<td>
<img style="width: 100%;" src="{{ site.baseurl }}/assets/images/research/autonomous/control_traditional.png">
</td>
</tr>  
<tr>
<td>
<div markdown="1">
- <b>Policy transfer</b> for reinforcement learning with robust control: *[Trans-ITS](https://ieeexplore.ieee.org/document/8924943)*, *[ITSC18](https://arxiv.org/abs/1812.03216)* *(**Best Student Paper**)*.
</div>
</td>
<td>
<div markdown="1">
- Our lab also published dozens of papers on vehicle dynamics and control over a decade ago, such as adaptive control ([*Trans-IE*](https://ieeexplore.ieee.org/document/1174058), [*ACC90*](https://ieeexplore.ieee.org/document/4791050)), adaptive cruise control ([*IJAT*](https://link.springer.com/article/10.1007/s12239-012-0007-6), [*IFAC*](https://www.sciencedirect.com/science/article/pii/S1474667016318390)), and control of truck with trailer ([*PATH-report*](https://www.researchgate.net/publication/46439115_Lateral_Control_of_Heavy_Duty_Vehicles_for_Automated_Highway_System_Experimental_Study_on_a_Tractor_Semi-trailer)).
</div>
</td>
</tr>  
</table>



## <a name="activity"></a>Activities


### Workshops & competitions in flagship conferences

##### Machine learning and computer vision community

- **[NeurIPS 2020](https://neurips.cc/) Competition** (December 2020) We organized a behavior prediction challenge in highly interactive driving scenarios, i.e., the  [INTERPRET Challenge](http://challenge.interaction-dataset.com/prediction-challenge/intro), as a regular competition at NeurIPS 2020. The [INTERACTION Dataset](https://interaction-dataset.com/) will be used in the challenge.
- **[CVPR 2020](http://cvpr2020.thecvf.com) Workshop** (June 2020) The results of the first round [INTERPRET Challenge](http://challenge.interaction-dataset.com/prediction-challenge/intro) will also be presented in CVPR 2020 Workshop organized by Waymo: [Scalability in Autonomous Driving](https://sites.google.com/view/cvpr20-scalability).
- **[ICML 2020](https://icml.cc/) Workshop** (July 2020) Wei Zhan was invited as a speaker to present the [INTERACTION Dataset](https://interaction-dataset.com/) and [INTERPRET Challenge](http://challenge.interaction-dataset.com/prediction-challenge/intro) in the ICML 2020 Workshop on [AI for Autonomous Driving](https://sites.google.com/view/aiad2020).

##### Robotics community

- **[RSS 2020](https://roboticsconference.org) Workshop** (June 2020): Interaction and Decision-Making in Autonomous-Driving, organized by Rowan McAllister, Liting Sun, Igor Gilitschenski, and Daniela Rus.
- **[IROS 2019](https://www.iros2019.org) Workshop** (Macao, November 2019): [Benchmark and Dataset for Probabilistic Prediction of Interactive Human Behavior](https://sites.google.com/berkeley.edu/iros2019-ws-dataset-benmark/home), organized by Wei Zhan, Liting Sun and Masayoshi Tomizuka.

##### Intelligent transportation/vehicle community

- **[IV 2020](https://2020.ieee-iv.org) Joint Workshops** (Las Vegas, postponed to October 2020): [From Benchmarking Behavior Prediction to Socially Compatible Behavior Generation in Autonomous Driving](https://sites.google.com/berkeley.edu/iv20-interaction/home), organized by Wei Zhan, Liting Sun, Maximilian Naumann, Jiachen Li and Masayoshi Tomizuka.
- **[ITSC 2020](https://www.ieee-itsc2020.org) Workshop** (September 2020): [Probabilistic Prediction and Comprehensible Motion Planning for Automated Vehicles – Approaches and Benchmarking](https://ieee-itsc2020.org/wp-content/uploads/2020/03/Probabilistic-Prediction-and-Comprehensible-Motion-Planning-for-Automated-Vehicles-–-Approaches-and-Benchmarking.pdf), organized by Maximilian Naumann, Martin Lauer, Liting Sun, Wei Zhan, Masayoshi Tomizuka, Arnaud de La Fortelle, Christoph Stiller.
- **[IV 2019](https://iv2019.org) Workshop** (Paris, June 2019): [Prediction and Decision Making for Socially Interactive Autonomous Driving](https://sites.google.com/berkeley.edu/iv19-interaction), organized by Wei Zhan, Jiachen Li, Liting Sun, Yeping Hu and Masayoshi Tomizuka.



## <a name="join"></a>Joining Our Group

Please send an email to Professor Masayoshi Tomizuka (tomizuka@berkeley.edu) and Dr. Wei Zhan (wzhan@berkeley.edu) if you are interested in our [Research Topics](#id4) and joining our group. 

- We are welcoming Berkeley students to directly work with us, or students out of Berkeley to visit us. We also accept virtual visit to work with us remotely for those with difficulties to conduct a physical visit. Please note that an experience will not be recognized without a formal interview and approval by the faculty and postdocs.
- For prospective Ph.D. students, please apply to the Mechanical Engineering Department of UC Berkeley by December 1st and send an email to address your strength and interest.

Please make sure that the following aspects are well covered in your application email. 

- Indicate in the email on your 1) primary goal of the research experience and particular interests; 2) start and end dates for working with us; 3) uniqueness and strength on research experiences/publications and/or skills and knowledge; 4) long-term/career goals.
- Attach a CV including your 1) home university, major, GPA and ranking; 2) research/working experiences; 3) publications/patents (if any); 4) skill set on coding/software/hardware and corresponding proficiency; 5) knowledge set on methods/algorithms.
- Attach a brief introduction (within 5 pages of slides) showing the core methods/algorithms and main results and demos of your previous research or working experiences. Links to cloud storage are welcome for large files.
- Attach all publications (including submitted paper) or well-formatted project final reports if any. Links to cloud storage or online publications are welcome.



## <a name="id5"></a>Members and Contact

The group lead is Dr. [Wei Zhan](https://scholar.google.com/citations?user=xVN3UxYAAAAJ&hl=en#). The research activities are coordinated by 2 Postdocs (Dr. [Wei Zhan](https://scholar.google.com/citations?user=xVN3UxYAAAAJ&hl=en#) and Dr. [Liting Sun](https://scholar.google.com/citations?user=BitIg-YAAAAJ&hl=en)) and conducted by 14 Ph.D. students (following headshots) with over 10 visiting researchers. 

<img width = "100%" src="{{ site.baseurl }}/assets/images/research/autonomous/headshots.png">

Please contact Dr. Wei Zhan (wzhan@berkeley.edu) and Professor Masayoshi Tomizuka (tomizuka@berkeley.edu) for more information if you are interested in the topics above by

- working with us (join/visit the group or collaborate) from academia, or
- research collaboration from industry.



