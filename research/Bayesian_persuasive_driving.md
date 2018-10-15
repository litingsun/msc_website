---
layout: page
title: Bayesian persuasive driving
permalink: /research/Bayesian_persuasive_driving.html
---

### Contents:

- [Introduction](#id1)

- [Publications](#id2)

- [Researchers](#id3)

  ​

## Bayesian persuasive driving



### <a name="id1"></a>Introduction

In the autonomous driving area, interaction between vehicles is still a piece of puzzle which has not been fully resolved. The ability to intelligently and safely interact with other vehicles can not only improve self driving quality but also be beneficial to the global driving environment. Although autonomous vehicles have been spotted more and more frequently driving on the city roads, most of them are still not interacting with other road users like human drivers do. Instead, most autonomous vehicles are implementing a reactive behavior, which means that the trajectory predictions about surrounding vehicles are made first and the ego vehicle's driving actions are decided accordingly by applying obstacle avoidance algorithm. However, in this planning pattern, the interaction between vehicles is ignored since the interacting vehicle's future driving profile is assumed to be independent of the ego vehicle's behavior. Therefore, more efforts are needed to fulfill a real interactive, efficient and cooperative driving environment where robot cars and human drivers coexist.

A promising optimization-based interactive planning approach is to formulate the interactive driving problem as a Bayesian persuasion game, which is first proposed for economic application. In the Bayesian persuasion game, there is one sender with information who attempts to persuade the receiver to change his/her action so that the welfare of both players can be improved. The basic assumptions include 1) the receiver's behavior is dependent on his/her belief of the world state and 2) both the players are rational Bayesian under which the interaction can be described as a Bayesian process. The persuasion process can be achieved by the sender via selecting certain information to convey to the receiver so that the receiver's posterior belief distribution of the world state can be properly manipulated.

In this work, a Bayesian persuasive driving algorithm based on optimization is proposed, where the ego vehicle is the persuader (information sender) and the surrounding vehicle is the persuadee (information receiver). In the persuasion process, the ego vehicle aims at changing the surrounding vehicle's posterior belief of the world state by providing certain information via signaling in order to achieve a lower cost for both players. The information received by the surrounding vehicle and its belief of the world state are described by Gaussian distributions. Concretely, the world state for the interactive driving environment is defined to be the ego vehicle's conservativeness perceived by the surrounding vehicle, the ego vehicle is defined as the information sender, whose information of driving intention can be reflected from his/her driving behavior and the surrounding interacting vehicle is the corresponding information receiver. With regard to the signal, several candidates are available including binary signal of yield or not yield, discrete signal of driving route selection and continuous signal of driving state. As a starting point, the ego vehicle's continuous driving state is selected as the signal since it carries the most driving information. By determining the optimal signal based on an optimization, the ego vehicle is able to achieve maximization/minimization of utility/cost expectation for both players. Meanwhile, the receiver will extract more information about the world state from the perceived signal and thus his/her posterior belief of the world state can be updated.

The following simulation results based on a 1/10 scaled test vehicle in several common traffic scenarios are provided, where the ego vehicle is the yellow one. It is shown that the proposed algorithm is capable of handling interaction situations involving surrounding vehicles with different driving characteristics.

<img width = "100%" src="{{ site.baseurl }}/assets/images/research/vehicle/Bayesian_persuasive_driving_lane_changing.png" >
<img width = "100%" src="{{ site.baseurl }}/assets/images/research/vehicle/Bayesian_persuasive_driving_lane_keeping.png" >
<img width = "100%" src="{{ site.baseurl }}/assets/images/research/vehicle/Bayesian_persuasive_driving_intersection.png" >

### <a name="id2"></a>Publications

Cheng Peng and Masayoshi Tomizuka, "[Bayesian Persuasive Driving](https://arxiv.org/abs/1809.09735)", submitted to <i>American Control Conference (ACC), 2019</i>.

Cheng Peng and Masayoshi Tomizuka, "[Cooperative Driving Based on Negotiation with Persuasion and Concession]", in <i>IEEE Intelligent Vehicles Symposium (IV), 2018</i>.



### <a name="id3"></a>Researchers

| Cheng Peng | Graduate Student | [Email Link](mailto:chengpeng2014@berkeley.edu)|