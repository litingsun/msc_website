---
layout: page
title: Autonomous Driving Via Imitation Learning and Optimization
permalink: /research/autonomous_driving_via_imitation_learning.html
---

### Contents:

* [Introduction](#id1)
* [Demo Videos](#id2)
* [Poster]({{ site.baseurl }}/assets/images/research/vehicle/Poster_imitation_learning_MPC.pdf)
* [Researchers](#id3)
* [Publications](#id4)

<!-- Title your work here -->

## Autonomous Driving Via Imitation Learning and Optimization


<!-- Add your own introduction here -->

### <a name="id1"></a>Introduction

Autonomous driving, as a convenience-enhancing technology, has attracted a great amount of research efforts in both academia and industry for its potential benefits on safety, accessibility, and efficiency.

Typically, autonomous driving systems are partitioned into hierarhical structures including perception, decision-making, motion planning and vehicle control. Among them, **planning and control** are two core yet challenging problems that are responsible for safety and efficiency. They should

1. comprehensively consider all possible constraints regarding safety and feasibility (kinematically and dynamically) based on the perceived environment in-formation and reasonable prediction of other roadparticipants’ behaviors;
2. generate optimal/near-optimal maneuvers that providegood driving qualities such as smoothness, passengers’ comfort and time-efficiency;
3. solve the problem within limited runtime to timely respond rapid changes in surrounding environment.

To simultaneously address the above challenges, we propose a two-layer hierarchical structure that combines imitation learning (Policy Layer) and optimization-based (Execuation Layer) methods, as shown below.

 <img src="{{ site.baseurl }}/assets/images/research/vehicle/overall_structure_v2.png" title="OverallStructure">

<div class="image-caption">The Hierarchical Structure of Learning-Optimization Based Autonomous Driving</div>



------

The *Policy Layer* in the hierarchical structure is represented by a neural network that is trained via imitation learning, and the *Execuation Layer* is a short-horizon optimization-based reference tracking controller. In the training phase, the expert data can come from either offline long-term optimization (for example, long-term Model Predictive Control, a.k.a, MPC) or real human driving data. In the test phase, the output of the *Policy Layer* is given to the *Execuation Layer* as an initial reference trajectory that the *Execuation Layer* will try to follow but with final check for collisions. Via such combination, we can generate a long-term trajectory with low collision probability and execute safely a short-term action fastly.

Moreover, to continuously improve the learning performance of the neural network in *Policy Layer* such that the long-term trajectory can be collision-free with higher and higher probability, we propose to use a *_Sampled DAgger_* process, as shown below.

 <img src="{{ site.baseurl }}/assets/images/research/vehicle/DAgger_procedure_v2.png"  width="20%" title="Dagger_procedure"/>

<div class="image-caption">The proposed Sampled DAgger procedure for continuous performance improvement</div>



------

### <a name="id2"></a>Demo Videos

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://youtube.com/embed/gEEOFyOStxk" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>

<div class="image-caption">Demos of autonomous driving via learning from optimization</div>

------

### <a name="id3"></a>Researchers

| Liting Sun | Graduate Student | [Email Link](mailto:litingsun@berkeley.edu) |	|
| Cheng Peng | Graduate Student | [Email Link](mailto:chengpeng2014@berkeley.edu) |  	|
| Wei Zhan | Graduate Student | [Email Link](mailto:wzhan@berkeley.edu)|  |

### <a name="id4"></a>Publications

L. Sun, C. Peng, W. Zhan, and M. Tomizuka, "[A Fast Integrated Planning and Control Framework for Autonomous Driving](https://arxiv.org/pdf/1707.02515.pdf)", in <i>arxiv, July, 2017</i>.