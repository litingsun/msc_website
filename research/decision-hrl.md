---
layout: page
title: Deep Hierarchical Reinforcement Learning for Decision-Making and Planning
permalink: /research/decision-hrl.html
---

### Contents:

* [Introduction](#id1)
* [Demo Videos](#id2)
* [Publication](#id3)
* [Researchers](#id4)

<!-- Title your work here -->

## Deep Hierarchical Reinforcement Learning for Decision-Making and Planning

<!-- Add your own introduction here -->

### <a name="id1"></a>Introduction

Deep reinforcement learning has achieved great progress recently in domains such as learning to play Atari games from raw pixel input. The model-free characteristics of reinforcement learning free us from hand-encoding complex policies. However, for real world tasks such as autonomous driving, there are some complex sequential decision making processes that contain distinct behaviors. Due to the delayed rewards and the averaged gradient, it is pretty difficult for a flat deep reinforcement learning algorithm to learn a good policy. 

Hierarchical reinforcement learning (HRL) introduces hierarchical structures into the policy. The key point of hierarchical reinforcement learning is to add temporal abstraction and intrinsic motivation. There are several great works in this field, such as MAXQ, option-critic, FeUdal network, modulated locomotor and MLSH. The success of these works on tackling difficult tasks proves that the method of temporal abstraction can significantly improve the performance of deep reinforcement learning. Using hierarchical policy can also benefit transfer learning, because the modularized policies can be easily reused in new tasks. Moreover, the decoupled policy modules enable us to get more interpretation of how the policy works.

In this research, we take advantage of the compositional characteristics of hierarchical reinforcement learning to separate these different behaviors into different policies. Then we train an additional master policy that can choose which behavior to execute with temporal abstraction. A policy gradient based hierarchical reinforcement learning algorithm is proposed to implement the method. The method is evaluated in a traffic light passing scenario simulation. The learned policy is analyzed with explicit interpretation, and the policy submodules can be reused in other scenarios.

### <a name="id2"></a>Demo Videos

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src=<iframe width="560" height="315" src="https://www.youtube.com/embed/jDFgh61Iqyg" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<div class="image-caption">Autonomous vehicle trained by deep hierarchical reinforcement learning passing a traffic light</div>

### <a name="id3"></a>Publication
J. Chen, Z. Wang and M. Tomizuka, “Deep Hierarchical Reinforcement Learning for Autonomous Driving with Distinct Behaviors”, in *2018 IEEE Intelligent Vehicles Symposium (IV)*.

### <a name="id4"></a>Researchers

| Jianyu Chen | Graduate Student | [Email Link](mailto:jianyuchen@berkeley.edu)|

| Zining Wang | Graduate Student | [Email Link](mailto:wangzining@berkeley.edu)|



