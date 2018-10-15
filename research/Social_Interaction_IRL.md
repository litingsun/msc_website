---
layout: page
title: Social Interaction-Aware Motion Planning for Autonomous Vehicles
permalink: /research/social_interaction_IRL.html

---

### Contents:

- [Introduction](#id1)
- [Demo Videos](#id2)
- [Researchers](#id3)
- [Publications](#id4)

<!-- Title your work here -->

<!-- Add your own introduction here -->

### <a name="id1"></a>Introduction

Autonomous cars are getting better at generating their motion not only in isolation, but also around people. We now have many strategies for dealing with interactions with people on the road, each modeling people in substantially different ways: starting as simple as assuming the person will maintain their current velocity within the planning horizon, to as complicated as learning a human driver policy or cost function, and model people as changing their plans depending on what the car does. 

Most of current works focus on **_how_** to optimize the robot's cost when the robot needs to interact with people. In this paper, we focus on **_what_**  the robot should optimize in such situations, particularly if we consider the fact that humans are not perfectly rational.

Typically, when designing the robot's cost function, we focus on safety and driving quality of the ego vehicle. Arguably, that is rather **_selfish_**. 

Selfishness has not been a problem with approaches that predict human plans and react to them, because that led to conservative robots that always try to stay out of the way and let people do what they want. But, as we are switching to more recent approaches that draw on the game-theoretic aspects of interaction, our cars are starting to become more aggressive. They cut people off, or inch forward at intersections to go first. While this behavior is good sometimes, we would not want to see it all the time. 

Our observation is that as we get better at solving the optimization problem for driving by better models of the world and of the people in it, there is an increased burden on the cost function we optimize to capture what we want. We propose that purely selfish robots that care about their safety and driving quality are not good enough. They should also be **_courteous_** to other drivers. This is of crucial importance since humans are not perfectly rational, and their behavior will be influenced by the aggressiveness of the robot cars.

*We advocate that a robot should balance minimizing the inconvenience it brings to another driver, and that we can formalize inconvenience as the increase in the other driver's cost due to the robot's behavior to capture one aspect of human behavior irrationality.*

In this work, we make the following contributions:

**A formalism for courtesy incorporating irrational human behavior.** We formalize courteous planning as trading off between the robot's selfish objective and a courtesy term, and introduce a mathematical definition for this term for irrational human behavior \--- we measure the increase of the vehicle's best cost under the robot's planned behavior, compared to the vehicle's best cost under an alternative "best case scenario", and define the cost increase as the courtesy term.

**An analysis of the effects of courteous planning.** We show the difference between courteous and selfish robots under different traffic scenarios. The courteous robot leaves the person more space when it merges, and might even block another agent (not a person) to ensure that the human can safely proceed.

\noindent\textbf{Showing that courtesy helps explain human driving.} We do an Inverse Reinforcement Learning (IRL)-based analysis to study whether our courtesy term helps in better predicting how humans drive. On the NGSIM dataset of real human driver trajectories, we find that courtesy produces trajectories that are significantly closer to the ground truth.

 <a name="id2"></a>Videos 

<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.3%;">
<iframe style = "position: absolute; width: 100%; height: 100%; left: 0; top: 0;"
  src="https://www.youtube.com/embed/DQNjaNGoX2g" frameborder="0" controls="controls" preload="auto" allowfullscreen></iframe>
</div>

------

### <a name="id3"></a>Researchers

| Liting Sun | Graduate Student | [Email Link](mailto:litingsun@berkeley.edu) |
| Wei Zhan | Graduate Student | [Email Link](mailto:wzhan@berkeley.edu)|

### <a name="id4"></a>Publications

L. Sun, W. Zhan, M. Tomizuka, and Anca D. Dragan, "[Courteous Autonomous Cars](https://arxiv.org/abs/1808.02633)", in proceedings of 2018 International Conference on Intelligent Robots (IROS), Oct 01-05, Madrid, Spain, 2018.