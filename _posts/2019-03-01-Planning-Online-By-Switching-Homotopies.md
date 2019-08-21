---
layout: post
title:  "[2019] Planning Online By Switching Homotopies (POSH)"
date: 2019-03-01 
description: An online planning algorithm to be presented at IROS 2019
---

This work was done in collaboration with Dr. Byron Boots and the Robot Learning Lab. The algorithm we developed, POSH, builds on previous work that frames the motion planning problem as one of optimizing a factor graph. While previous work focused on navigating a robot through a static environment, our work considers the case of an environment where the obstacles are moving around freely. POSH reoptimizes the factor graph representing the problem as the obstacles move, leading to a trajectory that evolves as the robot maneuvers around. The optimization is warm-started from the result of the previous solution and nodes in the graph that are no longer reachable are pruned away. This strategy allows the robot to switch the homotopy class of the trajectory it is following if the previous homotopy class becomes occluded. This approach reduces the frequence of collisions when compared to baselines that did not track solutions across multiple homotopies. The resulting paper: <a href="https://arxiv.org/abs/1908.00641">Online Motion Planning Over Multiple Homotopy Classes with Gaussian Process Inference</a> has been accepted to the IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS) 2019. 

<figure>
    <img src="{{ '/assets/img/posh.png' | prepend: site.baseurl }} " alt="">
</figure>
