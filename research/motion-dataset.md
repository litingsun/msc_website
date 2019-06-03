---
layout: page
title: Motion Dataset
permalink: /research/motion-dataset.html

---

### Contents:

- [Introduction](#id1)
- [Demo Videos](#id2)
- [Publications](#id3)
- [Download Link](#id4)
- [Researchers](#id5)

## A Vehicle Motion Dataset with Highly Interactive Driving Scenarios

### <a name="id1"></a>Introduction

Interactive vehicle motion dataset is an indispensable and fundamental asset for driving-behavior-related research areas, such as motion prediction, driver modeling, representation learning, imitation learning and social behavior generation, etc. Existing public vehicle motion datasets cannot meet the demands of these research areas on diversity, complexity and criticality of the interactive driving scenarios and behavior. Map information is also missing. We construct a vehicle motion dataset in a variety of highly interactive driving scenarios, including roundabouts, unsignalized intersections, ramp merging and double lane change. The interactive behavior of the vehicles in the selected scenarios are highly complex due to the relatively unstructured road, inexplicit right-of-way, as well as aggressive and irrational behavior caused by social pressures from other drivers. Critical situations can also be observed in the dataset, in which vehicles are nearly colliding. High-definition (HD) maps and reference paths are also provided in the dataset to generate key features to describe the motions. Our data processing pipeline and algorithms are developed with video stabilization, detection and tracking modules. The visualized results are provided for research on motion prediction, representation learning and human-like behavior generation utilizing the proposed dataset with corresponding map information. The results demonstrate how the dataset can facilitate driving-behavior-related research areas.

<!-- just change profile-placeholder.gif with an image of your choice. Don't forget to send the webmaster your picture as well. Be sure to fill out the data-title and title field of this tag -->

<img width = "60%" src="{{ site.baseurl }}/assets/images/research/vehicle/motion-dataset-illustration.png" title="Architecture">

<div class="image-caption">Detection results, tracking ID, and processed trajectories in round one minute.</div>

<!-- If you have any related work, then you can add them here. Be sure that you use this same template file to create those pages as well -->

### <a name="id2"></a>Demo Videos

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/9uzgj6Ep_ns" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>
<div class="image-caption">Diversity, complexity and criticality of the scenarios and behavior with examples of processed motion data.</div>

### <a name="id3"></a>Publications

W. Zhan, L. Sun, D. Wang, Y. Jin and M. Tomizuka, "A Vehicle Motion Dataset with Highly Interactive Driving Scenarios", submitted to <i>IROS 2019</i>.

### <a name="id4"></a>Download Link

Coming soon...

### <a name="id5"></a>Researchers

| Wei Zhan | Graduate Student |
| Liting Sun | Graduate Student |
| Di Wang | Visiting Student Researcher |
| Yinghan Jin | Visiting Student Researcher  |

| Masayoshi Tomizuka | Professor  |