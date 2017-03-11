---
layout: page
title: VIBRATION CONTROL OF INDUSTRIAL ROBOT
permalink: /research/vibration-suppression.html

---

### Contents:

* [Introduction](#id1)
* [Motion Control of Flexible Joint Robot](#id2)
* [Vibration Suppression of Flexible End-Effector](#id3)
* [Learning Control for Task Specific Industrial Robots](#id4)
* [Publications](#id5)
* [Sponsors](#id6)

<!-- Title your work here -->

## Vibration Control of Industrial Robot


<!-- Add your own introduction here -->

### <a name="id1"></a>Introduction

Precise motion control is desired in a variety of industrial robot applications. In order to 
achieve precise and rapid rest-to-rest motion, the overshoot and the residual vibration caused 
by flexibility of robots should be minimized. To make robot motion more accurate, several 
research topics are introduced, including motion control of flexible joint robot, vibration 
suppression of flexible end-effector , and learning control for task specific industrial robots.

<!-- just change profile-placeholder.gif with an image of your choice. Don't forget to send the webmaster your picture as well. Be sure to fill out the data-title and title field of this tag -->

### <a name="id2"></a>Motion Control of Flexible Joint Robot

This work try to improve trajectory tracking accuracy of robots with flexible joints. A 
MATLAB/SimMechanics simulator for 6-joint robot is developed. Both rigid body robot dynamics 
and joint flexibility effects are modelled in this simulator. For very soft joint, the 
simulation shows accutate trajectory tracking can be achieved using multiple sliding surface 
control (MSSC) that takes advantage of the model of robot dynamics and sensing from actuator 
and robot joints/links.

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/CvkO7m-aVaU" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
<div class="image-caption">Motion Control of Flexible Joint Robot</div>

<!-- If you have any related work, then you can add them here. Be sure that you use this same template file to create those pages as well -->

### <a name="id3"></a>Vibration Suppression of Flexible End-Effector

This work try to suppress vibration for robot with flexible payload / end-effector. The flexibility in flexible end-effector mainly comes from link flexibility. A modified input shaping technique, which is designed to work without slowing down the  shaped motion, is implemented in this work. Acceleration at the end tip of payload shows the performance of the vibration suppression.

<img width="800" src="{{ site.baseurl }}/assets/images/research/robot/RobotVibrationSuppression.png" title="experiment_setup_result">
<div class="image-caption">Hardware setup and experiment result</div>

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/OfwJjq4OWT4" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
<div class="image-caption">Vibration Suppression of Flexible End-Effector</div>


### <a name="id4"></a>Learning Control for Task Specific Industrial Robots

Iterative learning control (ILC) is a strategy that allows a control system to improve its performance by making use of the error signals collected from previous iterations. A prerequisite of using ILC is that the output reference has to be repetitive from trial to trial. A full run of ILC training (taking non-negligible time) is needed when there exist small changes in the reference signal. This paper introduces a new approach to extrapolate the converged ILC policies to previously unseen tracking problems. A time-frequency domain mapping is constructed to approximate the ILC policy for a group of trajectories used in a particular task, say spot welding. We also introduce the idea of feature-frequency space, where the ILC policies from different trajectories can be encoded into a single model. This model can generate a control policy that performs comparably to the ILC policy while having the advantage of not requiring a full training for a new trajectory. The proposed time-frequency domain feedforward learning (TFFL) method could achieve similar performance as the standard ILC.

<img width = "60%" src="{{ site.baseurl }}/assets/images/research/robot/learningControlCYL.png" title="learning_control">
<div class="image-caption">Learning Control for Task Specific Industrial Robots</div>


<!-- If you have researchers you want to list here, then fill out their name and title etc -->

### <a name="id5"></a>Publications

Y. Zhao, C. Wang, X. Yu, and M. Tomizuka, "[Complete Dynamic Modelling of Flexible Joint Robots](http://proceedings.asmedigitalcollection.asme.org/proceeding.aspx?articleid=2481910)," in <i>ASME Dynamic Systems and Control Conference (DSCC)</i>, 2015.

Y. Zhao, W. Chen, T. Tang, and M. Tomizuka, "[Zero Time Delay Input Shaping for Smooth Settling of Industrial Robots](http://ieeexplore.ieee.org/abstract/document/7743459/)," in <i> IEEE International Conference on Automation Science
and Engineering (CASE)</i>, 2016

C.-Y. Lin, W. Chen, and M. Tomizuka, "[Learning Control for Task Specific Industrial Robots](http://ieeexplore.ieee.org/document/7799380/)," in <i>IEEE Conference on Decision and Control (CDC)</i>, 2016

<!--| Yongxiang Fan | Graduate Student | [Email Link](mailto:yongxiang_fan@berkeley.edu) |  	|-->


<!-- If you have any sponsors, you can just list them here -->

### <a name="id6"></a>Sponsors

* [FANUC Corporation](http://www.fanuc.com/)