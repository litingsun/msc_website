---
layout: page
title: 'Safe OnGO-VIC: Online Gain Optimization for Variable Impedance Control with Control Barrier Functions'
permalink: /research/safe-ongo-vic.html
---

### Contents:

* [Abstract](#id1)
* [Videos](#id2)

<!-- Title your work here -->

<!-- Add your own introduction here -->

### <a name="id1"></a>Abstract

 Variable impedance control plays an importantrole in contact-rich manipulation tasks. It enables the robot to safely interact with unknown environments. In addition, it provides the flexibility to adapt the impedance according to different task goals and scenarios. While many studies focuses on designing the variable impedance control policies by adaptivecontrol and reinforcement learning methods, these approachesare typically over specific to one task and not time efficient to obtain. To deal with those problems, we present an efficient Safe Online Gain Optimization method for Variable Impedance Control (Safe OnGO-VIC). By reformulating the dynamics of impedance control as a control-affine system, in which the impedance gains are the inputs, we provide a new perspective to understand the variable impedance control and innovatively formulate an optimization problem for online gain adaptation. Moreover, control barrier  function (CBF) is incorporated into our gain optimization framework for safety guarantee. The proposed algorithm was experimentally validated on three manipulation tasks: 1) collision avoidance, 2) board contact, and 3) surface wiping. The comparison results with constant gain baseline and an adaptive control law in [1] prove that theproposed algorithm can achieve better performance efficiently, and it is more generalizable for different scenarios.

### <a name="id2"></a>Videos
<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe width="560" height="315" src="https://www.youtube.com/embed/CXpVS5jvlLs" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>