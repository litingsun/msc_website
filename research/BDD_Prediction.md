---
layout: page
title: Motion Generation and Cognition based on Deep Learning
permalink: /research/motion-generation.html
---

### Contents:

- [Introduction](#id1)

- [Publications](#id2)

- [Researchers](#id3)

- [Sponsors](#id4)

  ​

## Motion Generation and Cognition based on Deep Learning for Autonomous Driving



### <a name="id1"></a>Introduction

In this project, we tackle motion prediction and planning together as a motion generation problem to achieve accurate comprehension of others, as well as safe and human-like behavior generation for autonomous vehicles. Three major aspects are included in this project. First, Constrained Policy Net (CPN) was proposed to force a neural net to learn how to generate vehicle motions satisfying safety and feasibility constraints from an optimization-based expert planner. Second, we dive into inverse reinforcement learning to recognize intentions and predict motions of other road participants. Third, learning-based methods and conventional state estimation approaches are combined to deal with tracking and prediction problems in autonomous driving.

Policy networks have great potential to learn sophisticated driving policy under complicated interaction between human drivers. However, it is hard for policy networks to satisfy safety and feasibility constraints, which is not a challenging task for conventional motion generation methods, such as optimization-based approach. In this paper, we propose Constrained Policy Net (CPN), which can learn safe and feasible driving policy from arbitrary inequality-constrained optimization-based expert planners. Instead of supervised learning with $L_2$ norm as the loss, we incorporate the domain knowledge of the expert planner directly into the training loss of the policy net by applying barrier functions to the safety and feasibility constraints of the optimization problem. An exemplar scenario with obstacles on both sides is used to implement the proposed CPN. Test results demonstrate that the policy net can learn to generate motions near boundaries of safety and feasibility constraints to achieve high driving quality as the baseline optimization, while the constraints are satisfied.

<img width = "100%" src="{{ site.baseurl }}/assets/images/research/vehicle/visualizedNew.png" >
<div class="image-caption">Visualized motions of CPN compared with the baseline optimization and supervised learning</div>

Inverse Reinforcement Learning(IRL) is a powerful tool to tackle the problems of intention recognition and motion prediction. The main idea of IRL method is to learn the utilities and reward functions so that human-like behaviors can be generated via expert demonstration. In our research, we plan to derive the behavior of road participants by learning from a collection of real-world driving data under a variety of complicated scenarios in which interactions among multiple road participants are involved, such as busy roundabouts and four-way-stop intersections. The raw data from real-world driving are mainly point cloud from the Lidar, and dynamic occupancy grid methods would also be employed as a consistent representation of the data. The desired outputs are the intention of relevant road participants and predicted long-term motions.

Human-like motion generation is also a key to accurate object tracking, especially when the measurements from the sensors are lost or with low quality for a relatively long period. Since it is hard to accurately represent the state distribution by simple multivariate normal distributions, Particle Filter (PF) has advantages over other conventional state estimation techniques such as variants of Kalman Filter. When applied on tracking for autonomous driving, recursive state extimation techniques such as PF still have limitations. It is hard to formulate the system dynamics as precise stochastic models in different scenarios and simple system dynamics can lead to severe estimation uncertainty with low-quality or lost measurements for a long period. Also, Markov property is usually not satisfied. Therefore, we need to further explore advanced learning-based approaches, and combine them with conventional techniques to overcome these limitations and obtain better tracking performance.



### <a name="id2"></a>Publications

Wei Zhan, Jiachen Li, Yeping Hu, and Masayoshi Tomizuka, "[Safe and Feasible Motion Generation for Autonomous Driving via Constrained Policy Net](https://berkeley.box.com/v/CPN)", in <i>Annual Conference on IEEE Industrial Electronics Society (IECON), 2017</i>. 



### <a name="id3"></a>Researchers

| Jiachen Li | Graduate Student | [Email Link](mailto:wangzining@berkeley.edu)|

| Yeping Hu | Graduate Student | [Email Link](mailto:kiwoo.shin@berkeley.edu)|

| Wei Zhan | Graduate Student | [Email Link](mailto:wzhan@berkeley.edu) | 



### <a name="id4"></a>Sponsors

* [Berkeley Deep Drive](http://bdd.berkeley.edu)

