---
layout: post
title:  "[2018] Extending Homotopy-Based Shortest Path (HBSP)"
date: 2018-12-31 
description: A footstep planning algorithm for humanoids
---

During my time at <a href="https://riss.ri.cmu.edu">RISS</a> I collaborated with researchers at CMU to extend planning algorithms for humanoid robots. My work was on the HBSP (Homotopy Based Shortest Path) algorithm which  takes a given homotopy-class and generates a heuristic function to accelerate planning. We beat baseline methods (A* with a reverse Dijkstra Heuristic) by several orders of magnitude in environments with many local minima. My contribution to the project was extending the algorithm to work in "2.5 Dimensions" (i.e environments that cannot be projected into a single plane). This was done by extending the previous homotopy-invariants to encode 3-dimensional information. The resulting paper: <a href="https://arxiv.org/abs/1712.00531">Effective Footstep Planning Using Homotopy-Class Guidance</a> has been submitted to _Artifical Intelligence_ (an Elsevier journal). Our code is open sourced on <a href="https://github.com/vinitha910/homotopy_guided_footstep_planner">Github</a> for extension and application to other systems. 
<figure>
    <img src="{{ '/assets/img/hbsp.png' | prepend: site.baseurl }} " alt="">
</figure>
