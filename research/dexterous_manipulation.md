---
layout: page
title: REAL-TIME ROBUST FINGER GAITS PLANNING
permalink: /research/finger_gaits_planning.html

---

### Contents:

* [Introduction](#id1)
* [Algorithms](#id2)
* [Results](#id3)
* [Publications](#id4)
* [Researchers](#id5)

<!-- Title your work here -->

## Real-Time Robust Finger Gaits Planning under Object Shape and Dynamics Uncertainties


<!-- Add your own introduction here -->

### <a name="id1"></a>Introduction

Dexterous manipulation has broad applications in assembly lines, warehouses and agriculture. To perform large-scale manipulation tasks for various objects, a multi-fingered robotic hand sometimes has to sequentially adjust its grasping gestures, i.e. the finger gaits, to address the workspace limits and guarantee the object stability. However, realizing finger gaits planning in dexterous manipulation is challenging due to the complicated grasp quality metrics, uncertainties on object shapes and dynamics (mass and moment of inertia), and potential sliding under unknown contact dynamics. 
In this project, a dual-stage optimization based planner is proposed to handle these challenges. In the first stage, a velocity-level finger gaits planner is introduced by combining grasp quality with hand kinematic limitations. The proposed finger gaits planner is computationally efficient and realize finger gaiting without object 3D shape information. 
In the second stage, a robust manipulation controller using robust control and force optimization is proposed to address object dynamics uncertainties and external disturbances. The dual-stage planner is able to guarantee stability under potential sliding caused by unknown contact dynamics. Moreover, it does not require velocity measurement or expensive 3D/6D tactile sensors. Simulation results on Mujoco verify the proposed dual-stage optimization based planner. 

<!-- just change profile-placeholder.gif with an image of your choice. Don't forget to send the webmaster your picture as well. Be sure to fill out the data-title and title field of this tag -->



### <a name="id2"></a>Algorithms
The following figure shows the proposed dual-stage optimization based planner framework. First, grasp quality analysis is conducted by combining hand manipulability and object grasp quality, and the candidate breaking finger is chosen to change gait once the overall quality drops below a predefined threshold. A velocity-level finger gaits planner is evoked by this event, and the planner generates torque command to drive the selected finger towards the better quality region. The remaining fingers are controlled by a robust manipulation controller to generate desired torque, to manipulate the object stably and track the reference motion of the object. If the overall quality is above the threshold, all fingers will be controlled by the robust manipulation controller. 

A joint level torque tracking controller is used to track the desired torque command. The torque tracking controller uses a PID scheme and runs at a higher frequency, in comparison with the finger gaits planner and the robust manipulation controller (500 Hz).


<a href="{{ site.baseurl }}/assets/images/research/robot/grasp_algorithm.jpg" data-lightbox="Overview of Finger Gaiting Algorithm" data-title="Overview of Finger Gaiting Algorithm">
  <img src="{{ site.baseurl }}/assets/images/research/robot/grasp_algorithm.jpg" title="Overview of Finger Gaiting Algorithm">
</a>
<div class="image-caption">Overview of Finger Gaiting Algorithm</div>




<!-- If you have any related work, then you can add them here. Be sure that you use this same template file to create those pages as well -->

### <a name="id3"></a>Results

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/T-qW1hhhvSc" frameborder="0" controls="controls" preload="auto"></iframe>
</div>
<div class="image-caption">Real-Time Robust Finger Gaits Planning Under Object Shape and Dynamics Uncertainties
</div>


### <a name="id3"></a>Publications

1. Y. Fan, W. Gao, and M. Tomizuka, "Real-time finger gaits planning for dexterous manipulation," to appear in <i>The 20th World Congress of the International Federation of Automatic Control (IFAC)</i>, 2017.

2. Y. Fan, L. Sun, M. Zheng, W. Gao, and M. Tomizuka, "Robust dexterous manipulation under object dynamics uncertainties,"  submitted to <i>IEEE International Conference on Advanced Intelligent Mechatronics (AIM)</i>,
2017.

3. Y. Fan, T. Tang, H.-C. Lin, Y. Zhao, and M. Tomizuka, "Real-time robust finger gaits planning under object shape and dynamics uncertainties," submitted to <i>IEEE International Conference on Intelligent Robots and Systems (IROS)</i>, 2017.

<!-- If you have researchers you want to list here, then fill out their name and title etc -->

### <a name="id4"></a>Researcher

| Yongxiang Fan | Graduate Student | [Email Link](mailto:yongxiang_fan@berkeley.edu) |  	|



<!-- If you have any sponsors, you can just list them here -->
