---
layout: page
title: Building Temperature Control
permalink: /research/building-control
---

### Contents:

* [Introduction](#id1)
* [Research Topics](#id2)
* [Publications](#id4)
* [Researchers](#id3)

<!-- Title your work here -->

## Building Control


<!-- Add your own introduction here -->

### <a name="id1"></a>Introduction

Approximately, the buildings consume about 20-40% of the global energy, around half of which is used for heating, ventilation, and air conditioning system (HVAC). Therefore, it is necessary to consider advanced HVAC control strategies in order to reduce energy consumption and satisfy individuals' thermal comfort level demand at the same time. During the controller design process, both the outside environment disturbance and inside human activities should be considered. Although weather forecast and human activity schedule estimation could provide basic information of the disturbance, uncertainties still cannot be avoided. In addition, there are many constraints imposed by practical engineering system that need to be handled, including saturation constraint, stability constraint and so on.

<!-- just change profile-placeholder.gif with an image of your choice. Don't forget to send the webmaster your picture as well. Be sure to fill out the data-title and title field of this tag -->


<!-- If you have any related work, then you can add them here. Be sure that you use this same template file to create those pages as well -->

### <a name="id2"></a>Research Topics

Iterative design of feedforward and feedback controller

Note that for most commercial or residential buildings, there always exists some certain repetitive patterns for disturbance, including outside environment and inside human activities. With the repetitive nature of the disturbance, iterative learning control (ILC) is a suitable solution to consider. The central idea of ILC is to improve the performance of the current iteration based on learned information from previous iterations. Therefore, repetitive disturbance can be removed. In order to reduce the influence of non-repetitive components at the same time, an iterative tunable feedback controller is introduced. The control problem is formulated as an optimization problem. Through adjusting feedforward ILC signal and feedback controller iteratively, the control performance can be obviously improved.

<div class="container-fluid">
<div class="col-md-6">
<a href="{{ site.baseurl }}/assets/images/research/ILC_IFT.jpg" data-lightbox="ILC_IFT" data-title="ILC with IFT">
  <img src="{{ site.baseurl }}/assets/images/research/ILC_IFT.jpg" title="ILC with IFT">
</a>
<div class="image-caption">ILC with IFT design</div>
</div>

<div class="col-md-6">
<a href="{{ site.baseurl }}/assets/images/research/HVAC.jpg" data-lightbox="HVAC" data-title="HVAC system overview">
  <img src="{{ site.baseurl }}/assets/images/research/HVAC.jpg" title="HVAC system overview">
</a>
<div class="image-caption">HVAC System Overview</div>
</div>
</div>

<!-- If you have any related work, then you can add them here. Be sure that you use this same template file to create those pages as well -->

### <a name="id4"></a>Publications

1. C. Peng, W. Zhang and M. Tomizuka, "Iterative design of feedback and feedforward controller with input saturation constraint for building temperature control," 2016 American Control Conference (ACC), Boston, MA, 2016, pp. 1241-1246.
2. C. Peng, L. Sun, W. Zhang and M. TOmizuka, "Optimization-based constrained iterative learning control with application to building temperature control," 2016 Advanced Intelligent Mechatronics (AIM), Banff, Canada, 2016.

<!-- If you have researchers you want to list here, then fill out their name and title etc -->

### <a name="id3"></a>Researchers

| Cheng Peng | Graduate Student | [Email Link](chengpeng2014@berkeley.edu) |
| Shuyang Li | Graduate Student | [Email Link](shuyangli@berkeley.edu) |  	|