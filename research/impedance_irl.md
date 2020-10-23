---
layout: page
title: Learning Variable Impedance Control via Inverse Reinforcement Learning for Force-Related Tasks
permalink: /research/impedance-irl.html
---

### Contents:

* [Abstract](#id1)
* [Videos](#id2)

<!-- Title your work here -->

<!-- Add your own introduction here -->

### <a name="id1"></a>Abstract

Many manipulation tasks require robots to interact with unknown environments. In such applications, the ability to adapt the impedance according to different task phases and environment constraints is crucial for safety and performance Although many approaches based on deep reinforcement learning (RL) and learning from demonstration (LfD) have been proposed to obtain variable impedance skills on contact-rich manipulation tasks, these skills are typically task-specific and could be sensitive to changes in task settings. This paper proposes an inverse reinforcement learning (IRL) based approach to recover both the variable impedance policy and reward function from expert demonstrations. We explore different feature space of the reward functions to achieve a more general representation of expert variable impedance
skills. Experiments on two variable impedance tasks (Peg-in-Hole and Cup-on-Plate) were conducted in both simulation and
on a real FANUC LR Mate 200iD/7L industrial robot. The comparison results with behavior cloning and force-based IRL
proved that the learned reward function in gain action space has better transferability than in the force space.

### <a name="id2"></a>Videos
<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe width="560" height="315" src="https://www.youtube.com/embed/EQlQ6dAGHGU" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>