---
layout: page
title: Deep Neural Network for Semantic Intention and Motion
permalink: /research/prediction-simp.html
---

### Contents:

- [Introduction](#id1)

- [Demo Videos](#id2)

- [Publications](#id3)

- [Researchers](#id4)

  ​


## Probabilistic Prediction of Vehicle Semantic Intention and Motion



### <a name="id1"></a>Introduction


In this project, we focus on behavior predictions of traffic participants. The majority of current researches fix the number of driving intentions by considering only a specific scenario.  For example, manuvers such as lane keeping (LK), lane change left (LCL) and lane change right (LCR) are usually considered under non-junction segement like highway; for junction segement such as intersection, left turn, right turn, and go straight manuevers are involved. However, in order for autonomous vehicles to drive through dynamically changing traffic scenes in real life, an intention prediction module that can adapt to different scenarios with various possible driving maneuvers is necessary. To further improve the overall vehicle prediction performance, motion information is usually incorporated with classified intentions. As suggested in some literature, the methods that directly predict possible goal locations can achieve better performance for long-term motion prediction than other approaches due to their automatic incorporation of environment constraints. Moreover, by obtaining the temporal information of the predicted destinations, the optimal trajectories for predicted vehicles as well as the desirable path for ego autonomous vehicle could be easily generated.

We proposed a Semantic-based Intention and Motion Prediction (SIMP) method. It utilizes deep neural network to formulate a probabilistic framework which can predict the possible semantic intention and motion of the selected vehicle under various driving scenarios. The introduced semantics for this prediction problem is defined as answering the question of ”Which area will the predicted vehicle most likely insert into? Where and when?”, which incorporates both the goal position and the time information into each insertion area. Moreover, the adoption of probability can take into account the uncertainty of drivers as well as the evolution of the traffic situations.

The SIMP method is based on the structure of Mixture Density Nework(MDN). Mixture Density Network is a combination of ANN and mixture density model. The mixture density model can be used to estimate the underlying distribution of data, typically by assuming that each data point has some probability under a certain type of distribution. By using a mixture model, more flexibility can be given to model completely general conditional density function. Our task is to generate probability distributions of the designed semantic description given some representation of the current state. We assign a Gaussian Mixture Model (GMM) to each insertion area and multiple GMMs will be involved in one driving scenario. Each Gaussian mixture models the probability distribution of a certain type of motion for the predicted vehicle. Since obtaining the insertion location and the arriving time are the focus of our interests, a 2D Gaussian mixture is used and the predicted variables are constructed as a two dimensional vector.  We designed our loss function such that for the desired outputs, we expect not only the largest weight to be associated to the actual inserted area, but also the highest probability at the correct location and time for the output distributions of that area. 

An exemplar real-world scenario was used to implement and examine the proposed method. Below shows the testing results of two examplar cases. The full video can be found below. 

<img width = "100%" src="{{ site.baseurl }}/assets/images/research/vehicle/prediction-simp-test_cases.pdf" >

<div class="image-caption">Two example cases to visualize the performance.</div>

To further evaluate our method, the intention prediction and the motion prediction part were separately compared with two different baseline models: SVM and QRF. Our approach outperforms these methods in terms of both the prediction error and the confidence intervals. For more details, please check the paper linked below.  The key conclusion is that by combining different prediction tasks using semantics in a single framework, we can not only easily generalize the idea into any traffic scenarios but also obtain competitive performance compared to traditional methods. The output goal position and time information can be further used to generate optimal trajectories for predicted vehicles and eventually obtain a desirable path for our own autonomous vehicle. For future work, we will examine the SIMP method on more complex scenarios as well as take into account the occurrence of vehicle occlusion.

### <a name="id2"></a>Demo Videos

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
src="https://www.youtube.com/embed/6A3Hl-mRhbI" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>

<div class="image-caption">Visualization Results of NGSIM Testing Data</div>

### <a name="id3"></a>Publications

Y. Hu, W. Zhan and M. Tomizuka, "[Probabilistic Prediction of Vehicle Semantic Intention and Motion](https://arxiv.org/pdf/1804.03629.pdf)", in <i>2018 IEEE Intelligent Vehicles Symposium (IV)</i>. (**Best Student Paper Award**)



### <a name="id4"></a>Researchers

| Yeping Hu | Graduate Student | [Email Link](mailto:yeping_hu@berkeley.edu)|

| Wei Zhan | Graduate Student | [Email Link](mailto:wzhan@berkeley.edu) | 



