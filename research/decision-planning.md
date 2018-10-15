---
layout: page
title: Interaction-and-Uncertainty-Aware Joint Decision-Making and Planning
permalink: /research/decision-planning.html
---

### Contents:

* [Introduction](#id1)
* [Demo Videos](#id2)
* [Publication](#id3)
* [Researchers](#id4)

<!-- Title your work here -->

## Interaction-and-Uncertainty-Aware Joint Decision-Making and Planning

<!-- Add your own introduction here -->

### <a name="id1"></a>Introduction

Motivated by the potential social impact and fueled by the recent advances in both hardware (sensor technologies such as LIDAR) and software (artificial intelligence techniques such as deep learning), massive research efforts from industry and academy have been invested to autonomous driving for the last decades. Start from the DARPA urban challenges, a number of autonomous vehicle system demonstrations have been performed. Industry giant from automotive such as Toyota and Benz, IT such as Google and Uber, and startups are competing to develop the first commercialized fully autonomous vehicle.

Despite the inspiring achievements, there still exist bottlenecks on the path towards the true fully autonomous vehicle. The bottlenecks are caused by both the perception part and the planning part, making it extremely difficult to scaling up the current autonomous driving systems to handle the full open environment, while guaranteeing safety and maintaining efficiency. For perception, although deep learning techniques largely improved the performance for environment detection, it is not robust when encountered with scenarios that are quite different from those in the training set. For planning, there mainly exist the following challenges:

* Challenge 1: 
The decision making and motion planning for a autonomous driving system is typically hierarchically structured, with a high level decision making module to specify a local driving task, and a low level motion planning module to generate continuous trajectories. This framework brings several problems. First, there lacks a good communication between the two modules, the decision made might be difficult or not able for the planner to execute, which might result in serious safety problems. Second, The hierarchical structure requires recognition of scenario types and design of decision rules for each scenario, which makes it difficult to scale up. As various scenarios might happen at the same time, the system will be error prone.

* Challenge 2: 
Urban autonomous driving is difficult because the intention and future motion of surrounding vehicles are highly uncertain. However, current decision and planning system do not seriously consider the motion uncertainty and interactions. They often make simplifications of the surrounding vehicles' intentions and apply simple rules to handle them. The lack of an elaborate mechanism to handle the motion uncertainty will result in either too conservative or too aggressive actions.


In this research, we proposed an interaction-and-uncertainty-aware joint decision making and motion planning framework to tackle the above challenges, our work brings the following contributions:

* Contribution 1: 
A joint decision making and motion planning framework is constructed. Instead of sequentially make decisions and then plan motions to execute, we generate a pool of executable motions first. The decisions are then automatically classified by our method and taken into account when choosing the optimal motion. This joint framework avoids feasibility conflicts and provide more flexibility for us to analyze on both the decision level and the planning level. 

* Contribution 2: 
A mechanism is designed to handle the interaction with surrounding vehicles considering their motion uncertainty. The mechanism is naturally embedded to our joint decision making and motion planning framework. To this end, our system is able to make non-conservative and defensive plan for various scenarios. 

* Contribution 3: 
The whole system is performed in a generic and compact format we call the semantic map. It allows us to model any real world urban on-road driving scenario and then apply our algorithm on it.

### <a name="id2"></a>Demo Videos

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/Dpb0UV-dtEY" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<div class="image-caption">Autonomous vehicle entering a roundabout before the surrounding vehicle comes</div>

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/phmtWT0xwCU" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<div class="image-caption">Autonomous vehicle entering a roundabout while yielding to the surrounding vehicle</div>

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/dk7-OotihME" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<div class="image-caption">Autonomous vehicle entering a roundabout while the surrounding vehicle exiting</div>

### <a name="id3"></a>Publication
J. Chen, C. Tang, L. Xin, S. Li and M. Tomizuka, “Continuous Decision Making for On-road Autonomous Driving under Uncertain and Interactive Environments”, in *2018 IEEE Intelligent Vehicles Symposium (IV)*.


### <a name="id4"></a>Researchers

| Jianyu Chen | Graduate Student | [Email Link](mailto:jianyuchen@berkeley.edu)|

| Chen Tang | Graduate Student | [Email Link](mailto:chen_tang@berkeley.edu)|

| Long Xin | Visiting Student Researcher | [Email Link](mailto:long_xin@berkeley.edu)|

| Wei Zhan | Graduate Student | [Email Link](mailto:wzhan@mails.tsinghua.edu.cn)|


