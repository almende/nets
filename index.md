---
layout: default
title: Introduction
---

# Introduction

Nets contains all algorithms developed at Almende. Our algorithms are tailored for 
applications that have to do with networks. Networks (or nets) of humans, machines,
or (slightly exaggerated) neurons. Our research concerns the use of local mechanisms
to bring about global behaviour. However, besides that we also develop standard or
state-of-the-art techniques that have to do with concrete practical problems of 
machine learning, artificial intelligence, and networks of sensors, smartphones, and
robots. 

Our algorithms can be divided into several categories: 
- [Signal processing](#signalprocessing)
- [Classification](#classification)
- [Learning](#learning)
- [Planning](#planning)
- [Prediction](#prediction)

<!--
[<img src="img/dobots.png" 
  style="margin-top: 30px;" 
  title="Click for a larger view">](img/dobots.png)
-->

## Signal processing {#signalprocessing}

Nets contains many algorithms for signal processing and preprocessing which can be used
as basic functionality for classification, learning, and other higher-level tasks. There
are for example vision processing algorithms (such as optic flow calculations and basic
image feature extraction). 

- Links to this software will follow soon.

## Classification {#classification}

Nets contains several algorithms for classification. The requirements for robust 
classification stem from robotic platforms. We have hence classification methods
that are incremental opposed to batch-based. New data items can enter the classifier
in an incremental fashion rather than having all new data items available in for
example a file. This makes the software useful on robotics, or in real-time settings,
contrary to for example Hadoop or the Google Prediction API. However, what lacks yet
is to provide a nice online interface to have these classifiers used by third-parties.

Our current classifiers:

- [iLVQ](https://github.com/mrquincle/ilvq)
- [ARTMAP](https://github.com/mrquincle/artmap)

## Learning {#learning}

Nets provides algorithms for learning optimal policies in a general action-state 
space (the system normally represented by a POMDP, a Partial Observable Markov Decision
Process). Finding such optimal policies can be done by reinforcement learning and other
types of learning (for example using intrinsic reward rather than extrinsic reward).
The type of algorithms developed here can be used to have a group of robots vaccuum
a large office building as efficiently as possible, or to have a group of UAVs 
(unmanned aerial vehicles) search for a victim on sea or a fire in the dunes as 
quick as possible.

Our current learning methods:

- [Q-learning](https://github.com/mrquincle/actionperception)

With respect to learning it is important to note that our [classification](#classification) 
methods can be used in an unsupervised learning setting.

## Planning {#planning}

Nets provides currently no planning algorithms. With respect to planning as a decision
process, it is of course possible to use our [learning](#learning) algorithms.

## Prediction {#prediction}

Nets provides temporal classification algorithms and prediction algorithms. 

Our current prediction algorithms:

- [ESN](https://github.com/mrquincle/esn)


## Open source {#opensource}

Our algorithms are offered as open-source software under LGPLv3 or Apache license. Almende 
and spin-offs use it in their commercial products, which contribute to their maturity.
