---
layout: page
title: Probabilistic Prediction via Hierarchical Inverse Reinforcement Learning
permalink: /research/HIRL_prediction.html


---

### Contents:

- [Introduction](#id1)
- [Researchers](#id3)
- [Publications](#id4)

<!-- Title your work here -->

<!-- Add your own introduction here -->

### <a name="id1"></a>Introduction

#### Motivation

Autonomous vehicles (AVs) are interacting with human on the road. To this end, it needs to predict and reason about possible future behavior of human, and plan its own trajectories accordingly. Wrong prediction can cause either too conservative motions such as unnecessary stops/yielding, or dangerous situations like emergency brakes and unavoidable collisions. Hence, accurate prediction is of crucial importance to enable a safe and efficient autonomous car. 

Starting from as simple as assuming that the other drivers would maintain their current velocities within the planning horizon to as complicated as modelling the probability distributions over all possible trajectories/actions, many prediction approaches have been proposed. Most of them, however, formulate prediction in isolation, i.e., the influence of other vehicles' actions to the human driver is ignored.

In fact, human drivers will actively anticipate and reason about surrounding vehicles' behavior when they decide the next-step actions. This means that besides historical and current scene states, the distribution over all possible trajectories is also influenced by their beliefs about other vehicles' plan. For example, given the same historical trajectories, a lane-keeping driver might be more probable to decelerate rather than maintaining current speed if the driver believes that another vehicle is about to merge into his lane. The difference between **_Prediction in Isolation_** and **_Interaction-Aware Prediction_** are illustrated in Fig. 1.

 <img src="{{ site.baseurl }}/assets/images/research/vehicle/HIRL_isolated_vs_interaction_prediction.pdf" style="width:500px;height:400px;" title="Different prediction formulations">

<div class="image-caption">Fig. 1. Different formulations for prediction </div>

*Our insight is that in highly interactive driving scenarios, an accurate prediction should consider not only the time-domain dependency but also the interaction among vehicles. Namely, an autonomous car should anticipate the conditional probability over all possible trajectories of the human driver given not only historical and current states, but also its own future plans.*

#### Approach

To obtain such a probabilistic and interactive prediction of human drivers' behavior, we approximate the ``internal incentive'' of human via Inverse Reinforcement Learning. Moreover, noting that human's planning procedure is naturally hierarchical with both discrete and continuous driving decisions, we propose a **_hierarchical inverse reinforcement learning_** (IRL) framework. Given the autonomous vehicle's future plan, the probability distribution over all future trajectories of the predicted human driver is modelled as a mixture of distributions, partitioned by the discrete driving decisions. The example of the hierarchical structure is given in Fig. 2.

 <img src="{{ site.baseurl }}/assets/images/research/vehicle/HIRL_prediction_1.pdf" style="width:500px;height:550px;" title="hierarchical structure">

<div class="image-caption">Fig. 2. The probabilistic and hierarchical trajectory--generation process for a lane changing scenario </div>

#### Case Study

We collect 134 human driving trajectories in a freeway ramp-merging scenario from the Next Generation SIMulation (NGSIM) dataset. 80 of them are used for training, and the remaining 54 are for test. Figure 3 shows an examplar group of trajectories on the road map. There are four cars in scene, one merging vehicle (red), one lane-keeping vehicle (blue) and two surrounding vehicles (black), with one ahead of the blue car and the other behind. Our interest focuses on the interactive driving behavior of both the merging vehicle and the lane-keeping vehicle.

 <img src="{{ site.baseurl }}/assets/images/research/vehicle/HIRL_prediction_i80_map.pdf" title="I80 Map">

<div class="image-caption">Fig. 3. The merging map on Interstate 80 near Emeryville, California </div>

##### Training Performance

Figure 4 gives the training curves regarding to both the continuous and discrete driving decisions.  

 <img src="{{ site.baseurl }}/assets/images/research/vehicle/HIRL_prediction_all_training_curve.pdf" title="training curve">

<div class="image-caption">Fig. 4. The training curves of both the lane-keeping vehicle and the merging vehicle under different discrete driving decisions </div>

##### Test Performance

Prediction Performance among three approaches is compared: the proposed hierarchical IRL method, a neural-network (NN) based method and a hidden markov models (HMM) based method. 

A fatality-aware Brier score is adopted as an evaluation metric for the prediction of the discrete driving decisions. For the continuous driving trajectories, we use mean Euclidean distance as an evaluation metric. The results are shown in Table II and III.

 <img src="{{ site.baseurl }}/assets/images/research/vehicle/HIRL_prediction_Table_2.png" title="Discrete prediction performance">

 <img src="{{ site.baseurl }}/assets/images/research/vehicle/HIRL_prediction_Table_3.png" title="Continuous prediction performance">

<div class="image-caption">Table II and III. The performance of the proposed prediction algorithm </div>

Also, some examplar predicted trajectories as well as the corresponding ground-truth trajectories are given in Fig. 5. 

 <img src="{{ site.baseurl }}/assets/images/research/vehicle/HIRL_example_predicted_trajectories.pdf" title="training curve">

<div class="image-caption">Fig. 5. Three illustrative examples of the predicted most probable trajectories (red dotted line) compared with the ground truth trajectories (blue solid line). Thick black dash-dot lines represent the trajectories of other vehicles except for the predicted one. </div>

------

### <a name="id3"></a>Researchers

| Liting Sun | Graduate Student | [Email Link](mailto:litingsun@berkeley.edu) |
| Wei Zhan | Graduate Student | [Email Link](mailto:wzhan@berkeley.edu)|

### <a name="id4"></a>Publications

L. Sun, W. Zhan, and M. Tomizuka, "[Probabilistic Prediction of Interactive Driving Behavior via Hierarchical Inverse Reinforcement Learning](https://arxiv.org/abs/1809.02926)", to appear on the 21st IEEE International Conference on Intelligent Transportation Systems, November 4-7, 2018, Maui, Hawaii, USA.