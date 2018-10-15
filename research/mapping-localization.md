---
layout: page
title: Autonomous Vehicle Localization based on Multi-Sensor Fusion
permalink: /research/mapping-localization.html
---

### Contents:

* [Introduction](#id1)
* [Demo Videos](#id2)
* [Researchers](#id3)

<!-- Title your work here -->

## Vehicle Localization based on Multi-Sensor Fusion

<!-- Add your own introduction here -->

### <a name="id1"></a>Introduction

###Multi-sensor-based localization

Localization is a significant part for fully autonomous driving.  Insufficient positioning accuracy is one of the main problems that prevent the arrival of autonomous vehicle. The multi-sensor fusion based localization using global navigation satellite system (GNSS), inertial navigation system (INS), light detection and ranging (LiDAR) and high definition map (HD Map)  is well believed to be the final solution.  This project aims to provide globally referenced and accurate positioning service for autonomous vehicles  in diverse scenarios by taking the best of each sensors.

###Curb Detection

In urban scenes, curbs including guardrail, stones and bushes are significant features defining the physical drivable zones. Unlike lane-markings, the shapes of curbs are more flexible or irregular, which results in failures for the state-of-the-art curb detection methods. 

In this project, the off-line curb map building process is first performed which efficiently reduces the uncertainty during curb detection causing by false/missing detections. Afterwards, the on-line curb detection problem is formulated as a point set registration problem which involves noisy curb observation, noise-free curb map and IMU information. State estimation algorithms such as M-estimator, noise modelling and Kalman filter will be applied in corresponding section. 



### <a name="id2"></a>Demo Videos

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;" src="https://www.youtube.com/embed/ptmMR_-zD6Q" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>


<div class="image-caption">Map-aided Curb Detection</div>

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;" src="https://www.youtube.com/embed/1JR73LVlgqU" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>


<div class="image-caption">LiDAR-matching uncertainty estimation by capture the density of surrounding dynamic objects</div>

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;" src="https://www.youtube.com/embed/nRif4bQEMgU" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>


<div class="image-caption">Localization for autonomous vehicle using 3D LiDAR and pre-built point cloud map</div>

### <a name="id3"></a>Researchers

| Yiyang Zhou | Graduate Student | [Email Link](mailto:yiyang.zhou@berkeley.edu)|

| Weisong Wen | Visiting Student Researcher | [Email Link](mailto:17902061r@connect.polyu.hk)|

| Di Wang | Visiting Student Researcher | [Email Link](mailto:wenl14@mails.tsinghua.edu.cn)|

| Wei Zhan | Graduate Student | [Email Link](mailto:wzhan@berkeley.edu) | 


