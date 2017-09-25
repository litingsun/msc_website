---
layout: page
title: Decision-Making and Planning under Uncertainties with Social Interactions
permalink: /research/decision-making.html
---

### Contents:

- [Introduction](#id1)
- [Publications](#id2)
- [Posters](#id3)
- [Researchers](#id4)
- [Sponsors](#id5)



## Decision-Making and Planning under Uncertainties with Social Interactions for Autonomous Driving



### <a name="id1"></a>Introduction

Social interaction is an indispensable element in the real-world driving. The adherence to the underlying protocol keeps the traffic efficient, courteous, predictable and safe. However, the interactive prediction and planning were often omitted due to their theoretical, computational and empirical complexity, as well as the difficulty to quantify social factors. Such omission may lead to the conservative and unpredictable behaviors of autonomous vehicles, which may also jeopardize the safety. In this project, we are working on decision-making and planning under uncertainties by taking the social interaction into consideration to decrease the conservatism of the autonomous vehicle while guaranteeing it to survive in the worst case which may probably not happen. 

From the driving strategy point of view, a major challenge for autonomous vehicles in urban environment is to behave defensively to potential dangers, yet to not overreact to threats with low probability. A unified decision-making and planning framework under uncertainty is proposed, combining a decision network and an arbitrary motion planner with constraints, to achieve a non-conservatively defensive strategy (NCDS) in various kinds of scenarios. In the proposed framework, uncertainties from perception and behavioral predictions are simplified according to possible decision-making cases. Then we employ learning-based models to approximate the behavior of other road participants and obtain the threat probabilities of each case, including violations of the others. Also, a safe set is defined, which considers both current and preview safety. The proposed decision-making and planning framework is able to continuously adjust the short-term motion according to the threat probabilities, while safety is guaranteed in the worst case even if violations may exist.

Also, it is an indispensable building block for the major theme to propose a generic environmental representation and planning framework, which can deal with a variety of driving scenarios including extreme cases. Conventional layered planning architecture temporally partitions the spatiotemporal motion planning by the path and speed, which is not suitable for lane change and overtaking scenarios with moving obstacles. We propose to spatially partition the planning procedure by longitudinal and lateral motions along the rough reference path in the Frenet Frame, which makes it possible to create linearized safety constraints for each layer in a variety of on-road driving scenarios. A generic methodology for environmental representation is proposed with three topological elements and corresponding longitudinal constraints to compose all driving scenarios mentioned in this report according to the overlap between the potential path of the autonomous vehicle and the predicted path of other road users. Planners combining A* search and quadratic programming (QP) are designed to plan both long-term longitudinal motions and short-term trajectories to exploit the advantages of both search-based and optimization-based methods. Limits of vehicle kinematics and dynamics are considered in the planners to handle extreme cases. 



### <a name="id2"></a>Publications

Wei Zhan, Changliu Liu, Ching-Yao Chan, and Masayoshi Tomizuka, “[A Non-Conservatively Defensive Strategy for Urban Autonomous Driving](http://ieeexplore.ieee.org/abstract/document/7795595/)”, in <i>International IEEE Conference on Intelligent Transportation Systems (ITSC), 2016</i>. 

Wei Zhan, Jianyu Chen, Ching-Yao Chan, Changliu Liu and Masayoshi Tomizuka, “[Spatially-Partitioned Environmental Representation and Planning Architecture for On-Road Autonomous Driving](http://ieeexplore.ieee.org/document/7995789/)”,  in <i>IEEE Intelligent Vehicles Symposium (IV), 2017</i>. 

 Changliu Liu, Wei Zhan, and Masayoshi Tomizuka, “[Speed profile planning in dynamic environments via temporal optimization](http://ieeexplore.ieee.org/document/7995713/)”,  in <i>IEEE Intelligent Vehicles Symposium (IV), 2017</i>. 



### <a name="id3"></a>Posters

[A Non-Conservatively Defensive Strategy for Urban Autonomous Driving](https://berkeley.box.com/v/ncds-poster)

[Spatially-Partitioned Environmental Representation and Planning Architecture for On-Road Autonomous Driving](https://berkeley.box.com/v/iv2017-poster)



### <a name="id4"></a>Researchers

| Wei Zhan | Graduate Student | [Email Link](mailto:wzhan@berkeley.edu) | 



### <a name="id5"></a>Sponsors

* [International research Chair Drive for All](http://driveforall.com/)