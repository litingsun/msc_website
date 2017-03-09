---
layout: page
title: OBJECT POSE TRACKING FOR INDUSTRIAL MANIPULATORS
permalink: /research/object-pose-tracking.html
---

### Contents:

* [Introduction](#id1)
* [Algorithms](#id2)
* [Results](#id3)
* [Publications](#id4)
* [Researchers](#id5)
* [Sponsors](#id6)

<!-- Title your work here -->

## Object Position and Orientation Tracking for Manipulators Considering Nonnegligible Sensor Physics


<!-- Add your own introduction here -->

### <a name="id1"></a>Introduction

Real-time object tracking for manipulators has been broadly applied to industrial automation such as assembly and human robot collaboration. During the tracking process, the vision sensor is continuously treated as a feedback to the robot controller, which means the imperfect sensing and stability issues must be carefully considered. This paper deals with the sensing dynamics (i.e. limited sampling rate, irregular sampling time, packet loss, noise and latency), and realizes globally asymptotically stable tracking. First, an irregular time Kalman filter is employed to predict the states and covariances of feature points on the target, then the maximum likelihood technique is used to estimate the target pose from the distributions provided by the Kalman prediction. In addition, to realize object tracking, a dynamic tracking controller is presented and implemented. The stability of the system under model uncertainties is also discussed. The proposed tracking algorithm is verified in experiment.

<!-- just change profile-placeholder.gif with an image of your choice. Don't forget to send the webmaster your picture as well. Be sure to fill out the data-title and title field of this tag -->

The overall experimental setup is shown in the following figure. The PhaseSpace motion capture system is used as a vision sensor, and the experiment is implemented on FANUC LRMate 200iD/7L industrial manipulator. For simplification, the feature points are represented by markers. To mimic a general low cost commercial vision sensor, the sampling rate of PhaseSpace is down-sampled to 30 Hz,  while the controller reference generating rate is 125 Hz, and 30 percent of the vision data are discarded to mimic packet loss. The vision data is first sent to the host PC, and is further transmitted to target PC. During the transmission, other sensor physics such as latency and irregular sampling time are involved. The pose of the target is calculated by Kalman filter and maximum likelihood method in target PC. Then, the tracking controller computes the trajectory reference and the torque command and send it to the digital servo adapter (DSA). The robot controller connects DSA and robot and controls the robot according to signals from DSA. 


<img width = "60%" src="{{ site.baseurl }}/assets/images/research/robot/experiment_setup.jpg" title="experiment_setup">
<div class="image-caption">Experimental setup for object tracking</div>


### <a name="id2"></a>Algorithms

The control framework is shown in the following figure. First, the vision sensor detects the object and sends the position measurement of the markers. A general vision sensor has non-negligible sensor physics such as limited sampling rate, irregular sampling time, packet loss, noise and latency. 
Considering these challenges, we proposed a pose estimation algorithm. The pose estimation algorithm combines varying-rate Kalman filter and maximum likelihood technique. The varying-rate Kalman filter estimates the positions and the corresponding estimation variances of different markers. Then the maximum likelihood technique is used to estimate the position and orientation of the object based on the positions and variances of the marker estimations. A quaternion based tracking controller using both the kinematics and dynamics is presented to achieve globally asymptotically stable real-time visual tracking. 


<div>
<a href="{{ site.baseurl }}/assets/images/research/robot/control_framework.png" data-lightbox="The overall control framework" data-title="The overall control framework">
  <img src="{{ site.baseurl }}/assets/images/research/robot/control_framework.png" title="The overall control framework">
</a>
<div class="image-caption">The overall control framework</div>
</div>

<!-- If you have any related work, then you can add them here. Be sure that you use this same template file to create those pages as well -->

### <a name="id3"></a>Results

The experiment video is shown below. 

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/XpAYE7X76Xg" frameborder="0" controls="controls" preload="auto"></iframe>
</div>
<div class="image-caption">Experiment video for object position and orientation tracking</div>


### <a name="id3"></a>Publications

Y. Fan, H.-C. Lin, Y. Zhao, C.-Y. Lin, T. Tang, M. Tomizuka, and W. Chen, "Object position and orientation tracking for manipulators considering nonnegligible sensor physics," in  <i>Flexible Automation (ISFA), International Symposium on</i>. IEEE, 2016, pp. 450--457.

<!-- If you have researchers you want to list here, then fill out their name and title etc -->

### <a name="id4"></a>Researcher

| Yongxiang Fan | Graduate Student | [Email Link](mailto:yongxiang_fan@berkeley.edu) |  	|



<!-- If you have any sponsors, you can just list them here -->

### <a name="id5"></a>Sponsors

* [FANUC Corporation](http://www.fanuc.com/)