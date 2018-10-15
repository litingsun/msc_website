---
layout: page
title: Occluded Object Tracking based on Modiﬁed Mixture Particle Filter (MMPF)
permalink: /research/perception-pftracking.html
---

### Contents:

- [Introduction](#id1)

- [Demo Videos](#id2)

- [Publications](#id3)

- [Researchers](#id4)

  ​

## Occluded Object Tracking based on Modiﬁed Mixture Particle Filter (MMPF)



### <a name="id1"></a>Introduction
Accurate and robust tracking of surrounding road participants plays an important role in autonomous driving. However, there is usually no prior knowledge of the number of tracking targets due to object emergence, object disappearance and false alarms. To overcome this challenge, in this project we propose a generic vehicle tracking framework based on modified mixture particle filter, which can make the number of tracking targets adaptive to real-time observations and track all the vehicles within sensor range simultaneously in a uniform architecture without explicit data association. Each object corresponds to a mixture component whose distribution is non-parametric and approximated by particle hypotheses. Most tracking approaches employ vehicle kinematic models as the prediction model. However, it is hard for these models to make proper predictions when sensor measurements are lost or become low quality due to partial or complete occlusions. Moreover, these models are incapable of forecasting sudden maneuvers. To address these problems, we propose to incorporate learning-based behavioral models instead of pure vehicle kinematic models to realize prediction in the prior update of recursive Bayesian state estimation. Two typical driving scenarios including lane keeping and lane change are demonstrated to verify the effectiveness and accuracy of the proposed framework as well as the advantages of employing learning-based models.

Kalman filter (KF) is proved to be the optimal estimator for linear systems with Gaussian-distributed states and Extended Kalman filter (EKF) is utilized for non-linear systems. However, since it is hard to accurately represent the state distribution by simple multivariate Gaussian distributions in the real world, Particle filter (PF) has advantages over variants of Kalman filter since it has no limitations on the form of the system and state distributions.

Vehicle kinematic models are widely used as the state transition model at the prediction step in recursive state estimation. The simplest linear models are the Constant Velocity Model (CVM) and Constant Acceleration Model (CAM). More complicated models, such as Constant Steering Angle and Velocity Model (CSAVM) and Constant Steering Angle and Acceleration Model (CSAAM), take into account the correlation between the velocity and the yaw rate, which are also known as bicycle models [14]. Using these models can achieve encouraging tracking performance when sensor measurements are of high-quality. However, they are incapable of making long-term predictions when sensor measurements are lost or with low quality for a relatively long period. To deal with the problem, we propose
to enhance the capability of prediction models in addition to improving the detection algorithms.

In this work, we take advantage of a learning-based behavioral model in the proposed tracking framework as the system dynamics model for its capability of interacting with surrounding vehicles as well as learning to predict feasible and reasonable motions from real-world driving data. This approach has great advantages on tracking sudden maneuvers as well as reducing tracking variance. The learning-based models can also handle occlusions by short-term or long-term predictions.

<img width = "100%" src="{{ site.baseurl }}/assets/images/research/vehicle/perception-pftracking-tracking_1.png" >

<div class="image-caption"> Longitudinal Position and Velocity Tracking Results Comparison for Partial Occlusion (Lane Keeping)</div>

<img width = "100%" src="{{ site.baseurl }}/assets/images/research/vehicle/perception-pftracking-tracking_3.png" >

<div class="image-caption"> Longitudinal Position and Velocity Tracking Results Comparison for Complete Occlusion (Lane Keeping)</div>

<img width = "100%" src="{{ site.baseurl }}/assets/images/research/vehicle/perception-pftracking-tracking_2.png" >

<div class="image-caption"> Lateral / Longitudinal Position and Velocity Tracking Results Comparison for Partial Occlusion (Lane Change)</div>


### <a name="id2"></a>Demo Videos

<iframe width="560" height="315" src="https://www.youtube.com/embed/zbVQohw_uMc" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
<div class="image-caption"></div>




### <a name="id3"></a>Publications

Jiachen Li, Wei Zhan and Masayoshi Tomizuka, "[Generic Vehicle Tracking Framework Capable of Handling Occlusions Based on Modified Mixture Particle Filter](https://arxiv.org/pdf/1809.10237.pdf)", in <i>Proceedings of 2018 IEEE Intelligent Vehicles Symposium (IV), </i> 2018, pp. 936–942. 



### <a name="id4"></a>Researchers

| Jiachen Li | Graduate Student | [Email Link](mailto:jiachen_li@berkeley.edu)|

| Wei Zhan | Graduate Student | [Email Link](mailto:wzhan@berkeley.edu) | 


