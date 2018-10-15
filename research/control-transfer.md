---
layout: page
title: Deep Reinforcement Learning Driving Policy Transfer for Autonomous Vehicles
permalink: /research/control-transfer.html
---

### Contents:

- [Introduction](#id1)

- [Demo Videos](#id2)

- [Publication](#id3)

- [Researchers](#id4)


## Deep Reinforcement Learning Driving Policy Transfer for Autonomous Vehicles



### <a name="id1"></a>Introduction

Although deep reinforcement learning (deep RL) methods have lots of strengths that are favorable if applied to autonomous driving, real deep RL applications in autonomous driving have been slowed down by the modeling gap between the source (training) domain and the target (deployment) domain. Unlike current policy transfer approaches, which generally limit to the usage of uninterpretable neural network representations as the transferred features, in this project we propose to transfer concrete kinematic quantities in autonomous driving. The proposed robust-control-based (RC) generic transfer architecture, which we call RL-RC, incorporates a transferable hierarchical RL trajectory planner and a robust tracking controller based on disturbance observer (DOB). The architecture is shown in the figure below.

<img width = "100%" src="{{ site.baseurl }}/assets/images/research/vehicle/control-transfer-architecture.jpg" >

<div class="image-caption"> Reinforcement learning - robust controller policy transfer architecture</div>

The deep RL policies trained with known nominal dynamics model are transfered directly to the target domain, DOB-based robust tracking control is applied to tackle the modeling gap including the vehicle dynamics errors and the external disturbances such as side forces. Our simulations validating the capability of the proposed method to achieve zero-shot transfer across multiple driving scenarios such as lane keeping, lane changing and obstacle avoidance. The video is attached below. We have also transfered the lane keeping and lane changing policies to a real vehicle in Richmond Field Station.

### <a name="id2"></a>Demo Videos

<iframe width="560" height="315" src="https://www.youtube.com/embed/eOeuIUH0HAs" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
<div class="image-caption">Zero-shot RL Driving Policy Transfer for Autonomous Vehicles based on Robust Control</div>

### <a name="id3"></a>Publication

Z. Xu, C. Tang, and M. Tomizuka, "[Zero-shot Deep Reinforcement Learning Driving Policy Transfer for Autonomous Vehicles based on Robust Control]", in <i>IEEE International Conference on Intelligent Transportation Systems (ITSC), 2018</i>. 



### <a name="id4"></a>Researchers

| Zhuo Xu | Graduate Student | [Email Link](mailto:zhuoxu@berkeley.edu)|

| Chen Tang | Graduate Student | [Email Link](mailto:chen_tang@berkeley.edu)|


