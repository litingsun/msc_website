---
layout: page
title: Planning with Constrained Iterative LQR
permalink: /research/planning-cilqr.html
---

### Contents:

* [Introduction](#id1)
* [Demo Videos](#id2)
* [Publications](#id3)
* [Researchers](#id4)

<!-- Title your work here -->

## Planning with Constrained Iterative LQR

<!-- Add your own introduction here -->

### <a name="id1"></a>Introduction

Motion planning is a challenging area for autonomous driving. The planning module receives high-level decisions or behaviors from decision-making and behavior generation module, as well as a dynamic world model with road structure and states of all detected obstacles from perception module. The module finally generates trajectories satisfying safety and feasibility constraints with desirable driving quality. 

Typically, the representation of the constraints for collision avoidance in motion planners is relatively complex. Also, the trajectories need to be generated in a spatiotemporal domain in order to deal with highly dynamic driving scenarios, such as lane change and overtaking with moving obstacles. When generating motions in a spatiotemporal domain with a relatively long horizon, the computational load is often intractable so that the autonomous vehicle cannot respond to emergencies in real time. Therefore, autonomous vehicles need a motion planner which can 1) generate long-term motions in a spatiotemporal domain, 2) take into account complex collision avoidance constraints, as well as vehicle kinematic and dynamic models, and 3) achieve real-time computation so that emergency situations can be handled timely. 

Our approach utilizes the analytical expressions in Linear Quadratic Regulator (LQR) to design a motion planner with fast computation for complicated planning problems. Iterative LQR (ILQR) can be efficiently solved by dynamic programming (DP) to deal with unconstrained problems with non-quadratic objectives and nonlinear models. Constrained Iterative LQR (CILQR) is proposed in this paper to deal with constrained problems for motion planning of autonomous vehicles, so that the aforementioned requirements can be satisfied. The main contributions of this paper can be summarized as follows:

* New Fast Motion Planning Solver Proposed: 
We proposed a version of Constrained Iterative LQR algorithm to solve optimal control problems with nonlinear system dynamics and general form of constraints. We use logarithmic barrier function and introduce a new outer-inner loop framework to handle the constraints for Iterative LQR, achieving fast computation. 

* Convergence Property Proved:
The convergence of our proposed outer-inner loop iterative algorithm is proved in this paper, which guarantees the safety and performance of applying the algorithm.

* Applied to Autonomous Driving Problem Settings:
The proposed algorithm is then applied to an autonomous driving motion planning problem. The performance is evaluated with some challenging simulation scenarios.

### <a name="id2"></a>Demo Videos

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/Yivfd588l6s" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<div class="image-caption">Autonomous vehicle overtaking surrounding vehicles in multiple lanes</div>

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/uc3XBkji9-8" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<div class="image-caption">Autonomous vehicle accelerates to overtake the front vehicle before the upcoming vehicle on the opposite lane comes</div>

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/uw0QAiGd2nw" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<div class="image-caption">Autonomous vehicle decelerates to yield the upcoming vehicle on the opposite lane and then accelerates to overtake the front vehicle</div>

### <a name="id3"></a> Publications
J. Chen, W. Zhan, and M. Tomizuka, “Constrained Iterative LQR for On-Road Autonomous Driving Motion Planning”, in *2017 IEEE 20th International Conference on Intelligent Transportation Systems (ITSC)*, 2017, pp. 2232-2238.

J. Chen, W. Zhan, and M. Tomizuka, “Autonomous Driving Motion Planning with Constrained Iterative LQR”, submitted to *IEEE Transactions on Intelligent Vehicles*.

### <a name="id4"></a>Researchers

| Jianyu Chen | Graduate Student | [Email Link](mailto:jianyuchen@berkeley.edu)|

| Wei Zhan | Graduate Student | [Email Link](mailto:wzhan@berkeley.edu)|



