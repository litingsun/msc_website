---
layout: page-wide
title: Intelligent Control of Robotic Manipulators
permalink: /research/intelligent-manipulation.html
---

### Contents:

* [Introduction](#id1)
* [Research Topics](#id2)
* [Publications](#pb)
* [Researchers](#id3)
* [Recent Graduates](#id4)
* [Sponsors](#id5)

<!-- Title your work here -->

## Intelligent Control of Robotic Manipulators


<!-- Add your own introduction here -->

### <a name="id1"></a>Introduction

Designing high-performance, low-cost robot manipulators is one of the ultimate challenges for engineers today. Key performance criteria for these robots are: 1) cycling time, 2) accuracy and repeatability, 3) ease of programming, 4) intelligence and 5) safety. In striving to meet these increasingly stringent performance goals, a mechatronic approach, which combines aspects from both mechanical hardware and servo software, is required. This research focuses on vibration suppression, visual servoing, human robot collaboration and learning from demonstration. The project utilizes an integrated analytical, simulation, and experimental effort to attain the objectives.

<!-- just change profile-placeholder.gif with an image of your choice. Don't forget to send the webmaster your picture as well. Be sure to fill out the data-title and title field of this tag -->

<!-- If you have any related work, then you can add them here. Be sure that you use this same template file to create those pages as well -->

### <a name="id2"></a>Research Topics
<!-- Yu Zhao Edit -->
<table style="position:relative;">
<tr></tr><tr>
<td>
<div markdown="1">
* <b>Topic 1. Vibration Suppression</b>

Subtopic 1.1 Motion Control of Flexible Joint Robot
| [Brief](javascript:showhide("vib1")) | [More](javascript:toAppear()) |

</div>
<div id="vib1" style="display:none;">
This work try to improve trajectory tracking accuracy of robots with flexible joints. A MATLAB/SimMechanics simulator for 6-joint robot is developed. Both rigid body robot dynamics and joint flexibility effects are modelled in this simulator. For very soft joint, the simulation shows accutate trajectory tracking can be achieved using multiple sliding surface control (MSSC) that takes advantage of the model of robot dynamics and sensing from actuator and robot joints/links.
</div>

</td>
<td>
<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/CvkO7m-aVaU" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
<!--<div class="image-caption">Zero Time Delay Input Shaping</div>-->
</td>

<tr>
<td>
<div markdown="1">
* <b>Topic 1. Vibration Suppression</b>

Subtopic 1.2 Vibration Suppression of Flexible End-Effector
| [Brief](javascript:showhide("vib2")) | [More](javascript:toAppear()) |

</div>
<div id="vib2" style="display:none;">
This work try to suppress vibration for robot with flexible payload / end-effector. The flexibility in flexible end-effector mainly comes from link flexibility. A modified input shaping technique, which is designed to work without slowing down the shaped motion, is implemented in this work. Acceleration at the end tip of payload shows the performance of the vibration suppression.
</div>

</td>
<td>
<img src="{{ site.baseurl }}/assets/images/research/robot/RobotVibrationSuppression.png" title="Example Image">
<!--<div class="image-caption">Zero Time Delay Input Shaping</div>-->
</td>

<!-- Te, Hsien-Chung Edit -->
<tr>
<td>
<div markdown="1">
* <b>Topic 2. Robot Skill Learning</b>

Subtopic 2.1. Robot Learning from Human Demonstration with Remote Lead Through Teaching
| [Brief](javascript:showhide("skill1")) | [More](javascript:toAppear()) |
<div id="skill1" style="display: none;">
Industrial robots are playing increasingly important roles in factories. Many production applications require both position and force control; however, tuning the position-force controller is nontrivial. To simplify this process, the learning from demonstration (LfD) is proposed to transfer the human skills directly into robot applications. However, the current teaching methods, such as direct demonstration, lead through teaching, and teleoperation, all have their own drawbacks. Hence, Remote Lead Through Teaching (RLTT) is proposed to robot learn some tasks from human knowledge and skill. To implement the human skill model, the demonstration data is firstly synchronized by dynamic time warping (DTW), then decomposed into several actions by a support vector machine (SVM) based classifier. Lastly, the learning controller is trained by the Gaussian mixture regression (GMR). The experimental validation is realized on FANUC LR Mate 200iD/7L in an H7/h7 peg-hole insertion task and a surface grinding task.
</div>
</div>
</td>

<td>
<img width="60%" src="{{ site.baseurl }}/assets/images/research/robot/ECC.png" title="Example Image">
</td>

<tr>
<td>
<div markdown="1">
* <b>Topic 2. Robot Skill Learning</b>

Subtopic 2.2. Learn Peg-Hole-Insertion from Human Demonstration
| [Brief](javascript:showhide("skill2")) | [More](javascript:toAppear()) |
<div id="skill2" style="display: none;">
Programming robotic assembly tasks usually requires delicate force tuning. In contrast, human may accomplish assembly tasks with much less time and fewer trials. It will be a great benefit if robots can learn the human inherent skill of force control and apply it autonomously. Recent works on Learning from Demonstration (LfD) have shown the possibility to teach robots by human demonstration. The basic idea is to collect the force and corrective velocity that human applies during assembly, and then use them to regress a proper gain for the robot admittance controller. However, many of the LfD methods are tested on collaborative robots with compliant joints and relatively large assembly clearance. For industrial robots, the non-backdrivable mechanism and strict tolerance requirement make the assembly tasks more challenging. We modified the original LfD to be suitable for industrial robots. A new demonstration tool is designed to acquire the human demonstration data. The force control gains are learned by Gaussian Mixture Regression (GMR) and the closed-loop stability is analysed. A series of peg-hole-insertion experiments with H7h7 tolerance on a FANUC manipulator validate the performance of the proposed learning method.
</div>
</div>

</td>
<td>
<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/qNNLWfeePv4" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
<!--<div class="image-caption">Learn Peg-Hole-Insertion from Human Demonstration</div>-->
</td>


<tr>
<td>
<div markdown="1">
* <b>Topic 2. Robot Skill Learning</b>

Subtopic 2.3. Autonomous Alignment of Peg and Hole for Robotic Assembly
| [Brief](javascript:showhide("skill3")) | [More](javascript:toAppear()) |
<div id="skill3" style="display: none;">
In the past years, many methods have been developed for robotic peg-hole-insertion to automate the assembly process. However, many of them are based on the assumption that the peg and hole are well aligned before insertion starts. In practice, if there is a large pose(position/orientation) misalignment, the peg and hole may suffer from a three-point contact condition where the traditional assembly methods cannot work. To deal with this problem, we proposes an autonomous alignment method by force/torque measurement before insertion phase. A three-point contact model is built up and the pose misalignment between the peg and hole is estimated by force and geometric analysis. With the estimated values, the robot can autonomously correct the misalignment before applying traditional assembly methods to perform insertions. A series of experiments on a FANUC industrial robot and a H7h7 tolerance peg-hole testbed validate the effectiveness of the proposed method. Experimental results show that the robot is able to perform peg-hole-insertion from three-point contact conditions with 96% success rate. 
</div> 
</div>
</td>

<td>
<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/taZyWFny9xg" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
<!--<div class="image-caption">Autonomous Alignment of Peg and Hole for Robotic Assembly</div>-->
</td>

<!-- Changliu, Yujiao Edit -->
<tr>
<td>
<div markdown="1">
* <b>Topic 3. Human Robot Collaboration</b>

Subtopic 3.1. Human Guidance Programming with Collision Avoidance
| [Brief](javascript:showhide("HRI1")) | [More](javascript:toAppear()) |

<div id="HRI1" style="display: none;">
In the application of physical human-robot interaction (pHRI), the collaboration between human and robot can significantly improve the production efficiency through combination of the human's flexible intelligence and the robot's consistent performance. In this application, however, it is an important concern to ensure the safety of the human and the robot. In the human guidance programming scenario, the operator plans a collision-free path for the robot end-effector, but the robot body might collide with an obstacle while being guided by the operator. In this paper, a novel on-line velocity based collision avoidance algorithm is developed to solve the problem in this particular scenario. The proposed algorithm gives an explicit solution to deal with both collision avoidance and human guidance command at the same time, which provides the operator a better and safer lead through programming experience. The real-time experiment is performed on FANUC LR Mate 200iD/7L in three different obstacle scenarios.
</div>
</div>
</td>
<td>
	
<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/lqkp6g-RmxE" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>

</td>

<tr>
<td>
<div markdown="1">
* <b>Topic 3. Human Robot Collaboration</b>

Subtopic 3.2. Robot Safe Interaction System (RSIS)
| [Brief](javascript:showhide("HRI2")) | [More](javascript:toAppear()) |

<div id="HRI2" style="display: none;">
The long-term goal of this project is to establish a set of design principles of robot safe interaction systems (RSIS) which includes robust perception algorithms for environment monitoring and control algorithms for safe human robot interactions (HRI) of the intelligent co-robots. The proposed RSIS will prevent or minimize occurrences of human-robot collision and robot-robot collision. These algorithms, if applied to current co-robots, will significantly increase the operational speed of robots for higher productivity without sacrificing safety. 
</div>
</div>
</td>
<td>
<img src="{{ site.baseurl }}/assets/images/research/robot/collabration-HRI.jpg" title="Example Image">
</td>

<!-- Yongxiang Edit -->
<tr>
<td>
<div markdown="1">
* <b>Topic 4. Visual Tracking</b>  
| [Brief](javascript:showhide("vis")) | [More]({{ "/research/object-pose-tracking.html" | prepend: site.baseurl }}) |

</div>
<div id="vis" style="display: none;">
Real-time object tracking for manipulators has been broadly applied to industrial automation such as assembly and human robot collaboration. During the tracking process, the vision sensor is continuously treated as a feedback to the robot controller, which means the imperfect sensing and stability issues must be carefully considered. This paper deals with the sensing dynamics (i.e. limited sampling rate, irregular sampling time, packet loss, noise and latency), and realizes globally asymptotically stable tracking. First, an irregular time Kalman filter is employed to predict the states and covariances of feature points on the target, then the maximum likelihood technique is used to estimate the target pose from the distributions provided by the Kalman prediction. In addition, to realize object tracking, a dynamic tracking controller is presented and implemented. The stability of the system under model uncertainties is also discussed. The proposed tracking algorithm is verified in experiment.
</div>
</td>
<td>
<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/XpAYE7X76Xg" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
<!--<div class="image-caption">Experiment video for object position and orientation tracking</div>-->
</td>


<tr>
<td>
<div markdown="1">
* <b>Topic 5. Dexterious Manipulation</b>  
| [Brief](javascript:showhide("hand")) | [More]({{ "/research/finger_gaits_planning.html" | prepend: site.baseurl }}) |

</div>
<div id="hand" style="display: none;">
Dexterous manipulation has broad applications in assembly lines, warehouses and agriculture. To perform large-scale manipulation tasks for various objects, a multi-fingered robotic hand sometimes has to sequentially adjust its grasping gestures, i.e. the finger gaits, to address the workspace limits and guarantee the object stability. However, realizing finger gaits planning in dexterous manipulation is challenging due to the complicated grasp quality metrics, uncertainties on object shapes and dynamics (mass and moment of inertia), and potential sliding under unknown contact dynamics. 
In this project, a dual-stage optimization based planner is proposed to handle these challenges. In the first stage, a velocity-level finger gaits planner is introduced by combining grasp quality with hand kinematic limitations. The proposed finger gaits planner is computationally efficient and realize finger gaiting without object 3D shape information. 
In the second stage, a robust manipulation controller using robust control and force optimization is proposed to address object dynamics uncertainties and external disturbances. The dual-stage planner is able to guarantee stability under potential sliding caused by unknown contact dynamics. Moreover, it does not require velocity measurement or expensive 3D/6D tactile sensors. Simulation results on Mujoco verify the proposed dual-stage optimization based planner. </div>
</td>
<td>
<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/T-qW1hhhvSc" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
<!--<div class="image-caption">Experiment video for object position and orientation tracking</div>-->
</td>


<tr>
<td>
<div markdown="1">
* <b>Topic 6. Learning Control for Task Specific Industrial Robots</b>  
| [Brief](javascript:showhide("ILC")) | [More](javascript:toAppear()) |

</div>
<div id="ILC" style="display: none;">
Iterative learning control (ILC) is a strategy that allows a control system to im- prove its performance by making use of the error signals collected from previous iterations. A prerequisite of using ILC is that the output reference has to be repetitive from trial to trial. A full run of ILC training (taking non-negligible time) is needed when there exist small changes in the reference signal. This paper introduces a new approach to extrapolate the converged ILC policies to previously unseen tracking problems. A time-frequency domain mapping is con- structed to approximate the ILC policy for a group of trajectories used in a par- ticular task, say spot welding. We also introduce the idea of feature-frequency space, where the ILC policies from different trajectories can be encoded into a single model. This model can generate a control policy that performs compara- bly to the ILC policy while having the advantage of not requiring a full training for a new trajectory. The proposed time-frequency domain feedforward learning (TFFL) method could achieve similar performance as the standard ILC.</div>
</td>
<td>
<img width="70%" src="{{ site.baseurl }}/assets/images/research/robot/learningControlCYL.png" title="Example Image">

<!--<div class="image-caption">Experiment video for object position and orientation tracking</div>-->
</td>

<table></table>

<div markdown="1">

### <a name="pb"></a>Recent Publication

| T. Tang, C. Liu, W. Chen and M. Tomizuka, "[Robotic manipulation of deformable objects by tangent space mapping and non-rigid registration](http://ieeexplore.ieee.org/document/7759418/)," <i>2016 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)</i>, 2016. |
| H-C. Lin, Y. Fan, T. Tang, and M. Tomizuka, "[Human guidance programming on a 6-DoF robot with collision avoidance](http://ieeexplore.ieee.org/document/7759416/)," in <i>Intelligent Robots and Systems (IROS), 2016 IEEE/RSJ International Conference</i>. |
| T. Tang, H-C. Lin, Y. Zhao, W. Chen and M. Tomizuka, "[Autonomous alignment of peg and hole by force/torque measurement for robotic assembly](http://ieeexplore.ieee.org/document/7743375/)," <i>2016 IEEE International Conference on Automation Science and Engineering (CASE)</i>, 2016. (<b>Best Application Paper Finalist</b>) |
| T. Tang, H-C. Lin, Y. Zhao, Y. Fan, W. Chen and M. Tomizuka, "[Teach industrial robots peg-hole-insertion by human demonstration](http://ieeexplore.ieee.org/document/7576815/)," <i>2016 IEEE International Conference on Advanced Intelligent Mechatronics (AIM)</i>, 2016. |
| H-C. Lin, T. Tang, Y. Fan, Y. Zhao, M. Tomizuka, and W. Chen, "[Robot Learning from Human Demonstration with Remote Lead through Teaching](http://ieeexplore.ieee.org/abstract/document/7810316/)," in <i>European Control Conference (ECC)</i>, 2016. |
| C. Liu, and M. Tomizuka, "[Algorithmic safety measures for intelligent industrial co-robots](http://ieeexplore.ieee.org/abstract/document/7487476/)," in <i>IEEE International Conference on Robotics and Automation (ICRA), 2016. 
| Y. Fan, H.-C. Lin, Y. Zhao, C.-Y. Lin, T. Tang, M. Tomizuka, and W. Chen, "Object position and orientation tracking for manipulators considering nonnegligible sensor physics," in  <i>Flexible Automation (ISFA), International Symposium on</i>. IEEE, 2016, pp. 450--457. |
| Y. Fan, W. Gao, and M. Tomizuka, "Real-time finger gaits planning for dexterous manipulation," to appear in <i>The 20th World Congress of the International Federation of Automatic Control (IFAC)</i>, 2017. |
| Y. Fan, L. Sun, M. Zheng, W. Gao, and M. Tomizuka, "Robust dexterous manipulation under object dynamics uncertainties,"  submitted to <i>IEEE International Conference on Advanced Intelligent Mechatronics (AIM)</i>, 2017. |
| Y. Fan, T. Tang, H.-C. Lin, Y. Zhao, and M. Tomizuka, "Real-time robust finger gaits planning under object shape and dynamics uncertainties," submitted to <i>IEEE International Conference on Intelligent Robots and Systems (IROS)</i>, 2017. |
| Y. Zhao, C. Wang, X. Yu, and M. Tomizuka, "[Complete Dynamic Modelling of Flexible Joint Robots](http://proceedings.asmedigitalcollection.asme.org/proceeding.aspx?articleid=2481910)," in <i>ASME Dynamic Systems and Control Conference (DSCC)</i>, 2015. |
| Y. Zhao, W. Chen, T. Tang, and M. Tomizuka, "[Zero Time Delay Input Shaping for Smooth Settling of Industrial Robots](http://ieeexplore.ieee.org/abstract/document/7743459/)," in <i> IEEE International Conference on Automation Science and Engineering (CASE)</i>, 2016. |
| C.-Y. Lin, W. Chen, and M. Tomizuka, "Learning Control for Task Specific Industrial Robots," in <i>IEEE Conference on Decision and Control (CDC)</i>, 2016. |


<!-- If you have researchers you want to list here, then fill out their name and title etc -->

### <a name="id3"></a>Researchers

| Changliu Liu | Graduate Student | [Email Link](mailto:changliuliu@berkeley.edu) | [Homepage](http://www.me.berkeley.edu/~cliu/)	|
| Te Tang | Graduate Student | [Email Link](mailto:tetang@berkeley.edu) | [Homepage](http://www.me.berkeley.edu/~tetang/)  	 |
| Hsien-Chung Lin | Graduate Student | [Email Link](mailto:hclin@berkeley.edu)  | [Homepage](msc.berkeley.edu)	|
| Yu Zhao | Graduate Student | [Email Link](mailto:yzhao334@berkeley.edu) | [Homepage](msc.berkeley.edu)	|
| Yongxiang Fan | Graduate Student | [Email Link](mailto:yongxiang_fan@berkeley.edu)  | [Homepage](msc.berkeley.edu)	|
| Yujiao Cheng | Graduate Student | [Email Link](mailto:yujiaocheng@berkeley.edu) | |


### <a name="id4"></a>Recent Graduates

| Chung-Yen Lin | Apple | [Email Link](mailto:chung_yen@berkeley.edu) | 	|
| Cong Wang | NJIT | [Email Link](mailto:oski@berkeley.edy) |  |
| Michael Chan | Space X | [Email Link](javascript:brokenlink()) | |
| Pedro Reynoso | Nikon | [Email Link](javascript:brokenlink()) | |
| Wenjie Chen | FANUC | [Email Link](mailto:Chin.Bunketsu@fanuc.co.jp) |   |

<!-- If you have any sponsors, you can just list them here -->

### <a name="id5"></a>Sponsors

* [FANUC](http://www.fanuc.co.jp/eindex.htm)
</div>