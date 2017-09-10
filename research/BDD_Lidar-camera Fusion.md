---
layout: page
title: Lidar and Camera Fusion for 3D Object Detection based on Deep Learning
permalink: /research/lidar-camera-fusion.html
---

### Contents:

- [Introduction](#id1)
- [Videos](#id2)
- [Researchers](#id3)
- [Sponsors](#id4)
- [Acknowledgement](#id5)

## Lidar and Camera Fusion for 3D Object Detection based on Deep Learning for Autonomous Driving

<!-- Add your own introduction here -->

### <a name="id1"></a>Introduction

2D images from cameras provide rich texture descriptions of the surrounding, while depth is hard to obtain. On the other hand, 3D point cloud from Lidar can provide accurate depth and reflection intensity, but the solution is comparatively low. Therefore, 2D images and 3D point cloud are potentially supplementary to each other to accomplish accurate and robust perception, which is a prerequisite for autonomous driving.

Currently, there are several technical challenges in Lidar-camera fusion via convolutional neural network (CNN). Unlike RGB images for cameras, there is no standard input form for CNN from Lidars. Processing is required before fusing the 3D omnidirectional point cloud with the 2D front view images. The current region proposal networks (RPN), adapted from typical image processing structures, generate proposals separately and are not suitable for learning based on Lidar-camera fusion. Lidar-camera fusion enables accurate position and orientation estimation but the level of fusion in the network matters. Few works have been done on position estimation, and all existing works focus on vehicles.

In this project, our goal is to improve 3D object detection performance in driving environment by fusing 3D point cloud with 2D images via CNN. The RPN is applied to multiple layers of the whole network so that obstacles with different sizes in the front view are considered. We will be preprocessing Lidar and camera data from the KITTI benchmark and comparing the influence of Lidar data processing schemes by examining the contribution of Lidar information in detection. We will compare the region proposal accuracy in the form of 2D or 3D bounding boxes with other stereo-vision-based and fusion-based networks. Finally, we will collect data from real world traffic, pre-process and label the collected data according to the defined input and output of the CNN.



### <a name="id2"></a>Videos

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://youtube.com/embed/MMhQFThzHA4?rel=0" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>

<div class="image-caption">Point-cloud and corresponding image data collected with crowded pedestrains at a crosswalkr</div>



### <a name="id3"></a>Researchers

| Zining Wang | Graduate Student | [Email Link](mailto:wangzining@berkeley.edu)|

| Kiwoo Shin | Graduate Student | [Email Link](mailto:kiwoo.shin@berkeley.edu)|

| Wei Zhan | Graduate Student | [Email Link](mailto:wzhan@berkeley.edu) | 



### <a name="id4"></a>Sponsors

* [Berkeley Deep Drive](http://bdd.berkeley.edu)



### <a name="id5"></a>Acknowledgement

- We appreciate the help from Dr. Yi-Ta Chuang, Ehsan Javanmardi and Mahdi Javanmardi on data collection.