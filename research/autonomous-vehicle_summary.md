---
layout: page-wide
title: Autonomous Driving
permalink: /research/autonomous-vehicle.html
---

### Contents:

* [Introduction](#id1)
* [Research Topics](#id2)
* [Publications](#pb)
* [Researchers](#id3)


## Autonomous Driving

### <a name="id1"></a>Introduction

Our lab is focused on proposing novel methodologies and building corresponding facilities to solve the most challenging practical problems for full stack autonomous driving. We combine conventional control, planning and state estimation methods (optimal/robust control, optimization, graph search, Bayesian filtering, etc.) with state-of-the-art machine learning approaches (reinforcement learning, deep neural network, probabilistic graphical models, etc.) to exploit their advantages, and answer questions including but not limited to:

- How to combine conventional and learning-based methodologies for computationally efficient *planning and control* to achieve theoretical guarantee on stability, feasibility and safety, as well as flexibility to learn from trials and data?

- How to enable *decision-making and planning* under uncertainty with social interactions to achieve non-conservatively defensive driving strategies and persuade others to behave as we expected?

- What are good probabilistic predictions for reactions of other road users given our future decision, and how to provide accurate *probabilistic and reactive predictions* to enable safe decision-making and planning with desirable driving quality in a variety of highly interactive driving scenarios?

- How to fuse the information from multiple sensors to enable robust 3D object *detection and tracking* (with LIDAR and camera) and accurate large-scale *mapping and localization* (with LIDAR, GPS, IMU and camera)?

  <br>

### <a name="id2"></a>Research Topics

<!--  Edit -->

<table style="position:relative;">
<tr></tr>
    <tr>
<td>
<div markdown="1">
* <b> Motion Planning and Control </b> <br>


    1. Generic Environmental Representation and Planning  
    2. [Planning with Constrained Iterative LQR]({{"/research/planning-cilqr.html" | prepend: site.baseurl}})  
    3. Constrained Policy Net for Safe and Feasible Planning  
    4. [Planning and Control via Imitation Learning]({{"/research/autonomous_driving_via_imitation_learning.html" | prepend: site.baseurl}})    
    5. [Zero-Shot Deep Reinforcement Learning Policy Transfer based on Robust Control]({{"/research/control-transfer.html" | prepend: site.baseurl}})  

</div>



</td>
<td>

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://youtube.com/embed/RvjI4cpZAAE" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>


</td>

<!-- Edit -->
<tr>
<td>

<div markdown="1">
* <b> Decision-Making and Behavior Planning </b><br> 
    1. Non-Conservatively Defensive Strategy with Integrated Decision-Making and Planning  
    2. [Robustly-Safe Automated Driving (ROAD) System]({{"/research/robustly-safe-automated-driving.html" | prepend: site.baseurl}})  
    3. [Deep Hierarchical Reinforcement Learning for Decision-Making and Planning]({{"/research/decision-hrl.html" | prepend: site.baseurl}})  
    4. [Interaction-and-Uncertainty-Aware Joint Decision-Making and Planning]({{"/research/decision-planning.html" | prepend: site.baseurl}})  
    5. [Baysian Persuasive Driving]({{"/research/bayesian-persuasive.html" | prepend: site.baseurl}})
    6. [Inverse Reinforcement Learning for Social Interactions]({{"/research/social_interaction_IRL.html" | prepend: site.baseurl}})






</div>
</td>

<td>

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="http://www.youtube.com/embed/pvHaYfN7Ciw" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>

</td>



<!--  Edit -->

<tr>
<td>

<div markdown="1">
* <b> Prediction and Behavior Modeling </b><br>
Predicting the probabilistic behavior of others in highly interactive scenarios is one of the most challenging problems for autonomous driving. We propose novel methodologies based on deep neural networks, probabilistic graphical models and inverse reinforcement learning for interactive and probabilistic prediction problems. We also address the fundamental but under-explored aspects in the area of prediction, namely, problem formulation, representation simplification and evaluation metrics. Then we propose to construct a unified framework and fatality-aware benchmark to evaluate a variety of probabilistic reaction prediction algorithms.
    1. Fatality-Aware Benchmark for Probabilistic Reaction Prediction  
    2. [Inverse Reinforcement Learning for Social Interactions]({{"/research/social_interaction_IRL.html" | prepend: site.baseurl}})  
    3. [Hierarchical Inverse Reinforcement Learning for Probabilistic Prediction]({{"/research/HIRL_prediction.html" | prepend: site.baseurl}})  
    4. [Deep Neural Network for Semantic Intention and Motion]({{"/research/prediction-simp.html" | prepend: site.baseurl}})  
    5. [Situation Prediction based on Layered Hidden Markov Model]({{"/research/prediction-lhmm.html" | prepend: site.baseurl}})  
    6. [Generative Adversarial Network for Probabilistic Prediction]({{"/research/prediction-gan.html" | prepend: site.baseurl}})

</div>

</td>
<td>

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;"><iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"  src="https://www.youtube.com/embed/DQNjaNGoX2g" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe></div>


​			

<br>

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/6A3Hl-mRhbI" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>

</td>

<tr>
<td>

<div markdown="1">
* <b> Detection, Tracking, Localization and Mapping</b><br>
We are focused on LIDAR-Camera fusion for 3D object detection and tracking based on deep convolutional neural networks (CNN) for perception with onboard sensors. One of the models we proposed, RoarNet, was ranked **#2 on KITTI benchmark** for 3D car detection when submitted. When the object is partially or even fully occluded and the detection is noisy, we introduce learning-based behavioral prediction models combined with Bayesian filtering to achieve accurate tracking. We also investigate framework and methods to enable large-scale mapping and localization based on LIDAR, GPS, IMU and camera. 
    1. [Sparse Non-Homogeneous Pooling for CNN-based LIDAR-Camera Fusion]({{"/research/perception-pooling.html" | prepend: site.baseurl}})  
    2. [RoarNet: RegiOn Approximation Refinement for CNN-based LIDAR-Camera Fusion]({{"https://sites.google.com/berkeley.edu/roarnet"}})  
    3. [Occluded Object Tracking based on Modiﬁed Mixture Particle Filter]({{"/research/perception-pftracking.html" | prepend: site.baseurl}})  
    4. [Mapping and Localization based on Multi-Sensor Fusion]({{"/research/mapping-localization.html" | prepend: site.baseurl}})




</div>

</td>
<td>

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/CDp6mocT6C4" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
<br>

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/ZmnhvLlJ6qg" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
</td>

<table></table>

<div markdown="1">

### <a name="id3"></a>Recent Publications

J. Chen, W. Zhan, and M. Tomizuka, “Autonomous Driving Motion Planning with Constrained Iterative LQR”, submitted to *IEEE Transactions on Intelligent Vehicles*.

J. Li, H. Ma and Masayoshi Tomizuka, "Interaction-aware Multi-agent Tracking and Probabilistic Behavior Prediction via Adversarial Learning", submitted to ICRA 2019. 

K. Shin, Y. P. Kwon and M.Tomizuka, "[RoarNet: A Robust 3D Object Detection based on RegiOn Approximation Refinement](https://arxiv.org/abs/1811.03818)", submitted on ICRA 2019

C. Peng and M. Tomizuka, "[Bayesian Persuasive Driving](https://arxiv.org/abs/1809.09735)", submitted to <i>American Control Conference (ACC), 2019</i>.

W. Zhan, L. Sun, Y. Hu, J. Li, and M. Tomizuka, “[Towards a Fatality-Aware Benchmark of Probabilistic Reaction Prediction in Highly Interactive Driving Scenarios](https://arxiv.org/abs/1809.03478)”, in *2018 IEEE 21st International Conference on Intelligent Transportation Systems (ITSC)*, 2018.

L. Sun, W. Zhan, and M. Tomizuka, “[Probabilistic Prediction of Interactive Driving Behavior via Hierarchical Inverse Reinforcement Learning](https://arxiv.org/abs/1809.02926)'', in *2018 IEEE 21st International Conference on Intelligent Transportation Systems (ITSC)*, 2018.

Y. Hu, W. Zhan, and M. Tomizuka, “[A Framework for Probabilistic Generic Traffic Scene Prediction](https://arxiv.org/abs/1810.12506)”, in *2018 IEEE 21st International Conference on Intelligent Transportation Systems (ITSC)*, 2018.

J. Li, H. Ma, W. Zhan, and M. Tomizuka, “[Generic Probabilistic Interactive Situation Recognition and Prediction: From Virtual to Real](https://arxiv.org/abs/1809.02927)”, in *2018 IEEE 21st International Conference on Intelligent Transportation Systems (ITSC)*, 2018.

Z. Xu, C. Tang, and M. Tomizuka, "[Zero-shot Deep Reinforcement Learning Driving Policy Transfer for Autonomous Vehicles based on Robust Control](https://arxiv.org/abs/1812.03216v1)", in <i>IEEE International Conference on Intelligent Transportation Systems (ITSC), 2018</i>. (**Best Student Paper Award**)

L. Sun, W. Zhan, M. Tomizuka, and A. Dragan, “[Courteous Autonomous Cars](https://arxiv.org/abs/1808.02633)”, in *2018 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)*, 2018.

L. Sun, C. Peng, W. Zhan, and M. Tomizuka, “[A Fast Integrated Planning and Control Framework for Autonomous Driving](https://arxiv.org/pdf/1707.02515.pdf)”, in *ASME 2018 Dynamic System and Control Conference (DSCC)*, 2018.

W. Zhan, A. de La Fortelle, Y.-T. Chen, C.-Y. Chan, and M. Tomizuka, “[Probabilistic Prediction from Planning Perspective: Problem Formulation, Representation Simplification and Evaluation Metric](https://ieeexplore.ieee.org/abstract/document/8500697)”, in *2018 IEEE Intelligent Vehicles Symposium (IV)*, 2018, pp. 1150-1156.

Y. Hu, W. Zhan, and M. Tomizuka, “[Probabilistic Prediction of Vehicle Semantic Intention and Motion](https://arxiv.org/abs/1804.03629)”, in *2018 IEEE Intelligent Vehicles Symposium (IV)*, 2018, pp. 307-313. (**Best Student Paper Award**)

J. Li, W. Zhan, and M. Tomizuka, “[Generic Vehicle Tracking Framework Capable of Handling Occlusions Based on Modified Mixture Particle Filter](https://arxiv.org/abs/1809.10237)”, in *2018 IEEE Intelligent Vehicles Symposium (IV)*, 2018, pp. 936-942.

Z. Wang, W. Zhan, and M. Tomizuka, “[Fusing Bird-Eye View LIDAR Point Cloud and Front View Camera Image for 3D Object Detection](https://arxiv.org/abs/1711.06703)”, in *2018 IEEE Intelligent Vehicles Symposium (IV)*, 2018, pp. 834-839.

J. Chen, C. Tang, L. Xin, S. Li and M. Tomizuka, “[Continuous Decision Making for On-road Autonomous Driving under Uncertain and Interactive Environments](https://ieeexplore.ieee.org/abstract/document/8500605)”, in *2018 IEEE Intelligent Vehicles Symposium (IV)*.

J. Chen, Z. Wang and M. Tomizuka, “[Deep Hierarchical Reinforcement Learning for Autonomous Driving with Distinct Behaviors](https://ieeexplore.ieee.org/abstract/document/8500368)”, in *2018 IEEE Intelligent Vehicles Symposium (IV)*.

C. Peng and M. Tomizuka, "[Cooperative Driving Based on Negotiation with Persuasion and Concession](https://ieeexplore.ieee.org/abstract/document/8500702)", in <i>IEEE Intelligent Vehicles Symposium (IV), 2018</i>.

J. Chen, W. Zhan, and M. Tomizuka, “[Constrained Iterative LQR for On-Road Autonomous Driving Motion Planning](https://ieeexplore.ieee.org/abstract/document/8317745)”, in *2017 IEEE 20th International Conference on Intelligent Transportation Systems (ITSC)*, 2017, pp. 2232-2238.

W. Zhan, J. Li, Y. Hu, and M. Tomizuka, "[Safe and Feasible Motion Generation for Autonomous Driving via Constrained Policy Net](https://berkeley.box.com/v/CPN)", in <i>Annual Conference on IEEE Industrial Electronics Society (IECON), 2017</i>. 

C. Liu, W. Zhan, and M. Tomizuka, “[Speed profile planning in dynamic environments via temporal optimization](http://ieeexplore.ieee.org/document/7995713/)”,  in <i>IEEE Intelligent Vehicles Symposium (IV), 2017</i>. 

W. Zhan, J. Chen, C.-Y. Chan, C. Liu and M. Tomizuka, “[Spatially-Partitioned Environmental Representation and Planning Architecture for On-Road Autonomous Driving](http://ieeexplore.ieee.org/document/7995789/)”,  in <i>IEEE Intelligent Vehicles Symposium (IV), 2017</i>. 

C. Liu, J. Chen, T. Nguyen, and M. Tomizuka, "[The robustly-safe automated driving system for enhanced active safety](https://saemobilus.sae.org/content/2017-01-1406)", in <i>SAE World Congress, 2017</i>.

C. Liu, and M. Tomizuka, "[Enabling Safe Freeway Driving for Automated Vehicles](http://me.berkeley.edu/~cliu/files/acc16-2.pdf)", in <i>American Control Conference, 2016</i>. 

W. Zhan, C. Liu, Ching-Yao Chan, and M. Tomizuka, “[A Non-Conservatively Defensive Strategy for Urban Autonomous Driving](http://ieeexplore.ieee.org/abstract/document/7795595/)”, in <i>International IEEE Conference on Intelligent Transportation Systems (ITSC), 2016</i>. 

### <a name="id4"></a>Researchers

**Ph.D. Students**

 Wei Zhan | Graduate Student | [Email Link](mailto:wzhan@berkeley.edu) | 

 Cheng Peng | Graduate Student | [Email Link](mailto:chengpeng2014@berkeley.edu) | 

| Liting Sun | Graduate Student | [Email Link](mailto:litingsun@berkeley.edu) |
| Jianyu Chen | Graduate Student | [Email Link](mailto:jianyuchen@berkeley.edu)  |
| Zining Wang | Graduate Student | [Email Link](mailto:ziningwang@berkeley.edu) |
| Kiwoo Shin | Graduate Student | [Email Link](mailto:kiwoo.shi@berkeley.edu)  | 
| Jiachen Li | Graduate Student | [Email Link](mailto:jiachen_li@berkeley.edu)| 

| Yeping Hu | Graduate Student | [Email Link](mailto:yeping_hu@berkeley.edu)|

| Chen Tang | Graduate Student | [Email Link](mailto:chen_tang@berkeley.edu)|  

| Zhuo Xu | Graduate Student | [Email Link](mailto:zhuoxu@berkeley.edu)|  

| Hengbo Ma | Graduate Student | [Email Link](mailto:hengbo_ma@berkeley.edu)|  

| Lingfeng Sun | Graduate Student | [Email Link](mailto:lingfengsun@berkeley.edu)|  

| Yiyang Zhou | Graduate Student | [Email Link](mailto:yiyang.zhou@berkeley.edu)|  

**Recent Graduates**

| Changliu Liu | Carnegie Mellon University | 
| Shiying Zhou | Waymo | 

**Visiting Researchers**

| Hiroyuki Okuda | Visiting Scholar |

| Weisong Wen | Visiting Student Researcher | 

| Di Wang | Visiting Student Researcher | 

| Hyuntai Chin | Visiting Student Researcher | 

