---
layout: page
title: Sparse Non-homogeneous Pooling for Feature Map Fusion of LIDAR and Camera
permalink: /research/perception-pooling.html
---

### Contents:

- [Introduction](#id1)
- [Videos](#id3)
- [Researchers](#id4)

## Sparse Non-homogeneous Pooling for Feature Map Fusion of LIDAR and Camera

<!-- Add your own introduction here -->

### <a name="id1"></a>Introduction

This is the introduction of the extension of the published work [**Fusing Bird View LIDAR Point Cloud and Front View Camera Image for Deep Object Detection**](https://arxiv.org/abs/1711.06703). The code is released on the github [Sparse_Pooling](https://github.com/ZiningWang/Sparse_Pooling). The problem considered here is the feature fusion of different sensors in CNNs shown as the figure below

<img width = "100%" src="{{ site.baseurl }}/assets/images/research/vehicle/perception-pooling-Feature_and_Proposal_Fusion.png" >

<div class="image-caption"> Feature Fusion Network v.s. Proposal Fusion Network</div>

The fusion happens at the middle-stage which is of the best performance according to the Kitti Benchmark on July 23, 2018. The middle-stage fusion propose to fuse features after the convolution and down-sampling operations of the raw data and before the region proposal network (RPN). The fusion keeps the training of the network end-to-end.

<img width = "100%" src="{{ site.baseurl }}/assets/images/research/vehicle/perception-pooling-middle-stage-fusion.png" >

<div class="image-caption"> Different stages of fusion</div>

The main contributions of the Sparse Non-homogeneous Pooling Layer (SHPL) are:
#### Sparse Pooling Transforms and Preserves the Whole feature map
With the feature map preserved while the information of both sensors are fused, not only detection but also semantic segmentation and other tasks with fused features.  
One-stage detection framework can be utilized without RoI pooling which improves efficiency.  


#### Easy to Incorperate with Existing Networks and Very Little Overhead
The following figure shows the integration of SHPL with Avod-FPN. It improves the average precision (AP) by feature fusion, adding a subtle overhead to the mean inference time on the validation dataset.

<img width = "100%" src="{{ site.baseurl }}/assets/images/research/vehicle/perception-pooling-avod-fpn-SHPL-table.png" >

<div class="image-caption"> Avod-FPN-SHPL table</div>

<img width = "100%" src="{{ site.baseurl }}/assets/images/research/vehicle/perception-pooling-avod-fpn-with-SHPL.png" >

<div class="image-caption"> Avod-FPN-SHPL structure</div>

### <a name="id3"></a>Videos

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://youtube.com/embed/MMhQFThzHA4?rel=0" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>

<div class="image-caption">Point-cloud and corresponding image data collected with crowded pedestrains at a crosswalkr</div>



### <a name="id3"></a>Researchers

| Zining Wang | Graduate Student | [Email Link](mailto:wangzining@berkeley.edu)|

| Wei Zhan | Graduate Student | [Email Link](mailto:wzhan@berkeley.edu) | 



