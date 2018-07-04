---
layout: post
title:  "[2016] NN-Hyper-Octopus"
date: 2018-01-02 
description: My first project for Georgia Tech's ML club that sought to find the best learning rate given a network and data
---
Every semester, members of <a href="https://gtagency.github.io">The Agency</a>, the ML club at Georgia Tech work on projects to expose them to different fields of research in Machine Learning. My first semester in the club, I was working on a script for hyperparameter optimization. 

The idea was to use a genetic algorithm to optimize the learning rate parameter of a standard multilayer perceptron.  The learning rate decides how aggressively the weights of a network move in the direction of the gradient. The idea behind the genetic algorithm is that it spins up a "generation" of networks, the ones that have the lowest error after a fixed number of epochs are kept. These survivors are used to generate new learning rates for new networks. 

My contribution was writing the genetic algorithm, the training and architecture of the network was done by a teammate. The source is on <a href="https://github.com/gtagency/nn-hyper-octopus" target="_blank">Github</a>.
