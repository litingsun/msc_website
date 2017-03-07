---
layout: page
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

<div class="col-md-6">
<ahref="{{ site.baseurl }}/assets/images/profile-placeholder.gif" data-lightbox="profile-placeholder" data-title="Example Image">
  <img src="{{ site.baseurl }}/assets/images/profile-placeholder.gif" title="Example Image">


</a>
<div class="image-caption">FANUC Dual Robot Arm System (two 6-joint manipulator, force sensor, parallel gripper, MATLAB Simulink RealTime)</div>
</div>

<div class="col-md-6">
<a href="{{ site.baseurl }}/assets/images/profile-placeholder.gif" data-lightbox="profile-placeholder" data-title="Example Image">
  <img src="{{ site.baseurl }}/assets/images/profile-placeholder.gif" title="Example Image">

</a>
<div class="image-caption">FANUC Industrial Robot with Flexible Payload (controlled by MATLAB Simulink RealTime)</div>
</div>

<div class="col-md-6">
<a href="{{ site.baseurl }}/assets/images/profile-placeholder.gif" data-lightbox="profile-placeholder" data-title="Example Image">
  <img src="{{ site.baseurl }}/assets/images/profile-placeholder.gif" title="Example Image">
</a>
<div class="image-caption">Caption 2</div>
</div>






<!-- If you have any related work, then you can add them here. Be sure that you use this same template file to create those pages as well -->

### <a name="id2"></a>Research Topics


<!-- Yu Zhao Edit -->
1. Vibration Suppression

Precise motion control is desired in a variety of industrial robot applications. In order to achieve precise and rapid rest-to-rest motion, the overshoot and the residual vibration caused by flexibility of robots[7] should be minimized. Comparing to feedback control, feedforward is prefered since it does not affect the stability of the existing well tuned robot controller. Input shaping is well known for its simplicity and effectiveness for vibration suppression. However, the time delay introduced by input shaping is not desired in industrial robot applications since such delay would reduce the efficiency of production line. To solve this problem, modified input shaping approaches are developed. The time delay introduced by conventional input shaping technique can be fully compensated in the proposed approach [8]. 

<video width="100%" src="{{ site.baseurl }}/assets/images/research/robot/tobeUploadYZ.mp4" controls="controls" preload="auto"></video>
<div class="image-caption">Zero Time Delay Input Shaping
</div>



<!-- Te, Hsien-Chung Edit -->
2. Robot Skill Learning 

2.1 Remote Lead Through Teaching [1]
Many production applications require both position and force control; however, tuning the position-force controller is nontrivial. To simplify this process, Remote Lead Through Teaching (RLTT) is proposed to robot learn some tasks from human knowledge and skill. To establish the human skill model, the demonstration data is firstly synchronized by dynamic time warping (DTW), then decomposed into several actions by a support vector machine (SVM) based classifier. Lastly, the learning controller is trained by the Gaussian mixture regression (GMR). The experimental validation is realized on FANUC LR Mate 200iD/7L in a peg-hole insertion task and a surface grinding task.

2.2 Learn Peg-Hole-Insertion from Human Demonstration
Programming robotic assembly tasks usually requires delicate force tuning. In contrast, human may accomplish assembly tasks with much less time and fewer trials. It will be a great benefit if robots can learn the human inherent skill of force control and apply it autonomously. Recent works on Learning from Demonstration (LfD) have shown the possibility to teach robots by human demonstration. The basic idea is to collect the force and corrective velocity that human applies during assembly, and then use them to regress a proper gain for the robot admittance controller. However, many of the LfD methods are tested on collaborative robots with compliant joints and relatively large assembly clearance. For industrial robots, the non-backdrivable mechanism and strict tolerance requirement make the assembly tasks more challenging. We modified the original LfD to be suitable for industrial robots. A new demonstration tool is designed to acquire the human demonstration data. The force control gains are learned by Gaussian Mixture Regression (GMR) and the closed-loop stability is analysed. A series of peg-hole-insertion experiments with H7h7 tolerance on a FANUC manipulator validate the performance of the proposed learning method. [3]

<video width="100%" src="{{ site.baseurl }}/assets/images/research/robot/tobeUpload1.mp4" controls="controls" preload="auto"></video>
<div class="image-caption">Learn Peg-Hole-Insertion from Human Demonstration</div>


2.3 Autonomous Alignment of Peg and Hole for Robotic Assembly
In the past years, many methods have been developed for robotic peg-hole-insertion to automate the assembly process. However, many of them are based on the assumption that the peg and hole are well aligned before insertion starts. In practice, if there is a large pose(position/orientation) misalignment, the peg and hole may suffer from a three-point contact condition where the traditional assembly methods cannot work. To deal with this problem, we proposes an autonomous alignment method by force/torque measurement before insertion phase. A three-point contact model is built up and the pose misalignment between the peg and hole is estimated by force and geometric analysis. With the estimated values, the robot can autonomously correct the misalignment before applying traditional assembly methods to perform insertions. A series of experiments on a FANUC industrial robot and a H7h7 tolerance peg-hole testbed validate the effectiveness of the proposed method. Experimental results show that the robot is able to perform peg-hole-insertion from three-point contact conditions with 96% success rate. [2]     


<video width="100%" src="{{ site.baseurl }}/assets/images/research/robot/tobeUpload2.mp4" controls="controls" preload="auto"></video>
<div class="image-caption">Autonomous Alignment of Peg and Hole for Robotic Assembly
</div>


<video width="100%" src="https://www.youtube.com/watch?v=lqkp6g-RmxE" controls="controls" preload="auto"></video>
<div class="image-caption">Autonomous Alignment of Peg and Hole for Robotic Assembly
</div>




<!-- Changliu, Yujiao Edit -->

3. Human Robot Collaboration
-- Human Guidance Programming with Collision Avoidance [5]
In Human Robot Collaboration (HRC), it is an important concern to ensure the safety of the human and the robot. In the human guidance programming scenario, the operator plans a collision-free path for the robot end-effector, but the robot body might collide with an obstacle while being guided by the operator. To solve this problem, we propose a novel on-line velocity based collision avoidance algorithm, and implement a real-time experiment on FANUC LR Mate 200 iD/7L.




<!-- Yongxiang Edit -->

4. Visual Tracking

Real-time object tracking for manipulators has been applied to industrial automation such as assembly and human robot collaboration. During the tracking process, the vision sensor is used as a feedback means to the robot controller. It means that the imperfect sensing and stability issues must be carefully considered. This paper deals with the modeling of sensor physics (e.g. limited sampling rate, irregular sampling time, packet loss, noise, and latency), and realizes a globally asymptotically stable tracking controller. First, a varying rate Kalman filter is applied to estimate the markers’ positions and the corresponding error covariances. Then, a maximum likelihood estimation problem is solved to estimate the transformation between the target frame and the world frame. In addition, a dynamic tracking controller is implemented to realize object tracking. The stability of the tracking controller under model uncertainties is also discussed. The proposed tracking algorithm is experimentally verified on an industrial robot. [6]


<video width="100%" src="{{ site.baseurl }}/assets/images/research/robot/tracking_video.avi" controls="controls" preload="auto"></video>
<div class="image-caption">Experiment video for object position and orientation tracking
</div>



### <a name="pb"></a>Recent Publication
H-C. Lin, T. Tang, Y. Fan, Y. Zhao, M. Tomizuka, and W. Chen, "[Robot Learning from Human Demonstration with Remote Lead through Teaching](http://ieeexplore.ieee.org/abstract/document/7810316/)," in <i>European Control Conference (ECC)</i>, 2016. (<b>Best Application Paper Finalist</b>)

Te Tang, Hsien-Chung Lin, Yu Zhao, Wenjie Chen, and Masayoshi Tomizuka, "Autonomous Alignment of Peg and Hole by Force/Torque Measurement for Robotic Assembly," the 12th Conference on Automation Science and Engineering (CASE, ISAM 2016), Fort Worth, TX, USA, August 21-24, 2016. (Best Application Paper Finalist)

Te Tang, Hsien-Chung Lin, Yu Zhao, Yongxiang Fan, Wenjie Chen, and Masayoshi Tomizuka, "Teach Industrial Robots Peg-Hole-Insertion by Human Demonstration," the 2016 IEEE/ASME International Conference on Advanced Intelligent Mechatronics (AIM), Banff, Alberta, Canada, July 12-15, 2016.

Te Tang, Changliu Liu, Wenjie Chen, and Masayoshi Tomizuka, "Robotic Manipulation of Deformable Objects by Tangent Space Mapping and Non-Rigid Registration," the 2016 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), Deajeon, Korea, October 9-14, 2016.

Hsien-Chung Lin, Yongxiang Fan, Te Tang, and Masayoshi Tomizuka, "Human Guidance Programming on a 6-DoF robot with Collision Avoidance," the 2016 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), Deajeon, Korea, October 9-14, 2016.

Yongxiang Fan, Hsien-Chung Lin, Yu Zhao, Chung-Yen Lin, Te Tang, Masayoshi Tomizuka, and Wenjie Chen, "Object Position and Orientation Tracking for Manipulators Considering Unnegligible Sensor Physics," the 2016 International Symposium on Flexible Automation (ISFA), Cleveland, USA, August 1-3, 2016.

Yu Zhao, Cong Wang, Xiaowen Yu, and Masayoshi Tomizuka, "Complete Dynamic Modelling of Flexible Joint Robots," the 2015 ASME Dynamic Systems and Control Conference (DSCC), Columbus, Ohio, USA, October 28-30, 2015.

Yu Zhao, Wenjie Chen, Te Tang, and Masayoshi Tomizuka, "Zero Time Delay Input Shaping for Smooth Settling of Industrial Robots," the 12th Conference on Automation Science and Engineering (CASE, ISAM 2016), Fort Worth, TX, USA, August 21-24, 2016.


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
| Michael Chan | Space X | [Email Link]() | |
| Pedro Reynoso | Nikon | [Email Link]() | |
| Wenjie Chen | FANUC | [Email Link](mailto:Chin.Bunketsu@fanuc.co.jp) |   |

<!-- If you have any sponsors, you can just list them here -->

### <a name="id5"></a>Sponsors

* [FANUC](http://www.fanuc.co.jp/eindex.htm)