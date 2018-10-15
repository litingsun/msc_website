---
layout: page
title: Generative Adversarial Network for Probabilistic Prediction
permalink: /research/prediction-gan.html
---

### Contents:

- [Introduction](#id1)

- [Publications](#id2)

- [Researchers](#id3)


## Generative Adversarial Network for Probabilistic Prediction


### <a name="id1"></a>Introduction
In order for appropriate and high-quality decision making and motion planning of intelligent agent systems such as intelligent robotics and autonomous vehicles, accurate
probabilistic predictions for surrounding interactive objects is a crucial prerequisite. Although many research studies have been devoted to make predictions on a single entity, it remains an open challenge to forecast future behaviors for multiple interactive agents simultaneously. In this work, we take advantage of the Generative Adversarial Network (GAN) due to its capability of distribution learning and propose a generic multi-agent probabilistic prediction and tracking framework which takes the interactions among multiple entities into account, in which all the entities are treated as a whole. However, since GAN is very hard to train, we make an empirical research and present the relationship between training stability, training performance and hyperparameter values with a numerical case study. The results imply that the proposed model can capture both the mean, variance and multi-modalities of groundtruth distribution. Moreover, we apply the proposed approach to a real-world vehicle tracking and behavior prediction task to demonstrate its effectiveness and accuracy. The results illustrate that the proposed model trained by adversarial learning can achieve a better prediction performance than other state-of-the-art models trained by traditional supervised learning which maximizes the data likelihood. The well-trained model can also be utilized as an implicit proposal distribution for particle filtered based Bayesian state estimation which can improve tracking accuracy.



### <a name="id2"></a>Publications

J. Li, H. Ma and Masayoshi Tomizuka, "Interaction-aware Multi-agent Tracking and Probabilistic Behavior Prediction via Adversarial Learning", submitted on ICRA 2019. 



### <a name="id3"></a>Researchers

| Jiachen Li | Graduate Student | [Email Link](mailto:jiachen_li@berkeley.edu)|

| Hengbo Ma | Graduate Student | [Email Link](mailto:hengbo_ma@berkeley.edu)|



