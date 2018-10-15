---
layout: page
title: Situation Prediction based on Layered Hidden Markov Model
permalink: /research/prediction-lhmm.html
---

### Contents:

- [Introduction](#id1)

- [Publications](#id2)

- [Researchers](#id3)

  ​


## Situation Prediction based on Layered Hidden Markov Model


### <a name="id1"></a>Introduction
Accurate and robust recognition and prediction of traffic situation plays an important role in autonomous driving, which is a prerequisite for risk assessment and effective
decision making. Although there exist a lot of works dealing with modeling driver behavior of a single object, it remains a challenge to make predictions for multiple highly interactive agents that react to each other simultaneously. In this project, we propose a generic probabilistic hierarchical recognition and prediction framework which employs a two-layer Hidden Markov Model (TLHMM) to obtain the distribution of potential situations and a learning-based dynamic scene evolution model to sample a group of future trajectories. Instead of predicting motions of a single entity, we propose to get the joint distribution by modeling multiple interactive agents as a whole system. Moreover, due to the decoupling property of the layered structure, our model is suitable for knowledge transfer from simulation to real world applications as well as among different traffic scenarios, which can reduce the computational efforts of training and the demand for a large data amount. A case study of highway ramp merging scenario is demonstrated to verify the effectiveness and accuracy of the proposed framework.

The hierarchical recognition and prediction framework consists of two modules: situation recognition module and interactive scene evolution module. The recognition model has a two-layer structure which is a cascade of two groups of canonical HMM. The inference output of the first layer is utilized as the observation sequences of the second layer. Each HMM in the first layer corresponds to a certain low-level stage of situation evolution while each HMM in the second layer corresponds to a high-level situation which consists of several low-level stages and covers a relatively long period. Learning-based models can be employed to predict a longterm scene evolution. First, a prediction model is learned for each potential situation from the corresponding training data. Then, we can utilize each prediction model to generate a group of trajectories for each objective entities based on the posterior distributions obtained in the recognition module.

<img width = "100%" src="{{ site.baseurl }}/assets/images/research/vehicle/prediction-lhmm-LHMM_1.png" >

<div class="image-caption"> Typical traffic scenarios that lead to strong interaction among vehicles: (a) highway entrance; (b) roundabout; (c) uncontrolled T-intersection. The figures come from the bird-view of several road modules of the driving simulator developed by the authors.</div>

<img width = "100%" src="{{ site.baseurl }}/assets/images/research/vehicle/prediction-lhmm-LHMM_4.png" >

<div class="image-caption"> A simplified diagram of highway ramp merging process. </div>

<img width = "100%" src="{{ site.baseurl }}/assets/images/research/vehicle/prediction-lhmm-LHMM_2.png" >

<div class="image-caption"> The inference output of recognition module for three test case: (a) The main lane car yields the merging car; (b) The merging car yields the main lane car; (c) The merging car tends to cut in ahead of the main lane car while the main lane car does not yield. (a-1), (b-1) and (c-1) show the first-layer HMM inference output; and (a-2), (b-2) and (c-2) show the probability output of the second-layer HMM for ”main lane car yields”.</div>

<img width = "100%" src="{{ site.baseurl }}/assets/images/research/vehicle/prediction-lhmm-LHMM_3.png" >

<div class="image-caption"> An illustrative heatmap of long-term dynamic scene evolution. It contains predictions of the same case from the same initial state with different
propagation length. The red line is the ground truth of the merging vehicle and the blue line is the ground truth of the main lane vehicle. </div>



### <a name="id2"></a>Publications

Jiachen Li, Hengbo Ma, Wei Zhan and Masayoshi Tomizuka, "[Generic Probabilistic Interactive Situation Recognition and Prediction: From Virtual to Real](https://arxiv.org/pdf/1809.02927.pdf)", in <i>Proceedings of 2018 IEEE Intelligent Transportation Systems Conference (ITSC), </i> IEEE, 2018. 



### <a name="id3"></a>Researchers

| Jiachen Li | Graduate Student | [Email Link](mailto:jiachen_li@berkeley.edu)|

| Hengbo Ma | Graduate Student | [Email Link](mailto:hengbo_ma@berkeley.edu)|

| Wei Zhan | Graduate Student | [Email Link](mailto:wzhan@berkeley.edu) | 


