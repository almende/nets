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
- [Reasoning](#reasoning)

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

Our signal processing suite will contain (besides image processing facilities) procedures
like [principle component analysis](http://en.wikipedia.org/wiki/Principal_components_analysis),
[independent component analysis](http://en.wikipedia.org/wiki/Independent_component_analysis),
[singular value decomposition](http://en.wikipedia.org/wiki/Singular_value_decomposition), and
other pretty standard techniques.

Our current signal processing software:

- [ORB feature descriptor](https://github.com/mrquincle/aim_modules/KeypointModule) 

## Classification {#classification}

Nets contains several algorithms for classification. The requirements for robust 
classification stem from robotic platforms. We have hence classification methods
that are incremental opposed to batch-based. New data items can enter the classifier
in an incremental fashion rather than having all new data items available in for
example a file. This makes the software useful on robotics, or in real-time settings,
contrary to for example Hadoop or the Google Prediction API. However, what lacks yet
is to provide a nice online interface to have these classifiers used by third-parties.

Our repository of classifiers will be extended in the near future with for example the
[support vector machine](http://en.wikipedia.org/wiki/Support_vector_machine), the
[naive Bayes classifier](http://en.wikipedia.org/wiki/Naive_Bayes_classifier), and
[multilayer perceptrons](http://en.wikipedia.org/wiki/Multilayer_perceptron).

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

The type of algorithms to be exected are [reinforcement learning](http://en.wikipedia.org/wiki/Reinforcement_learning)
and variants like [Q-learning](http://en.wikipedia.org/wiki/Q_learning), [SARSA](http://en.wikipedia.org/wiki/SARSA) and [temporal difference learning](http://en.wikipedia.org/wiki/Temporal_difference_learning). 

Another series of algorithms are meant for state estimation, such as the [Kalman filter](http://en.wikipedia.org/wiki/Kalman_filter) 
(and variants such as the ensemble and unscented), and the [particle filter](http://en.wikipedia.org/wiki/Particle_filter).

In robotics the combination of state estimation (of the position of the robot itself) and
learning (of a map) is called [SLAM](http://en.wikipedia.org/wiki/Simultaneous_localization_and_mapping) 
(Simultaneous Localisation And Mapping). Incremental versions of SLAM are of interest to us.

Last, but not least, unsupervised learning methods, such as [k-means clustering](http://en.wikipedia.org/wiki/K-means_clustering),
[slow feature analysis](http://en.wikipedia.org/wiki/Principal_components_analysis), will be
included.

Our current learning methods:

- [Particle filter](https://github.com/mrquincle/particlefilter)
- [Q-learning](https://github.com/mrquincle/actionperception)

With respect to learning it is important to note that our [classification](#classification) 
methods can be used in an unsupervised learning setting.

## Planning {#planning}

Nets provides currently no planning algorithms. With respect to planning as a decision
process, it is of course possible to use our [learning](#learning) algorithms. 

## Prediction {#prediction}

Nets provides temporal classification algorithms and prediction algorithms. In other words,
everything that has something to do with time.

Our algorithms will be - as always - concentrated around incremental and/or decentralised
approaches. And will entail [model predictive control](http://en.wikipedia.org/wiki/Model_predictive_control),
[reservoir computing](http://en.wikipedia.org/wiki/Reservoir_computing), and for example
[conditional random fields](http://en.wikipedia.org/wiki/Conditional_random_field).

Our current prediction algorithms:

- [ESN](https://github.com/mrquincle/esn)

## Reasoning {#reasoning}

Reasoning is perhaps not a task that is quickly associated with networks of entities, but 
advances in especially probabilistic graphical models have introduced a lot of synergies
between Markov decision processes, Bayesian inference, and stochastic optimal control, to
name a few.

Our algorithms will entail [belief propagation](http://en.wikipedia.org/wiki/Belief_propagation),
[variational methods](http://en.wikipedia.org/wiki/Variational_Bayesian_methods) (a generalized
version of [expectation-maximization](http://en.wikipedia.org/wiki/Expectation-maximization)) 
and other algorithms of a similar taste.

Our current reasoning algorithms:

- [Belief Propagation](https://github.com/mrquincle/aim_modules/BeliefModule)

## Open source {#opensource}

Our algorithms are offered as open-source software under LGPLv3 or Apache license. Almende 
and spin-offs use it in their commercial products, which contribute to their maturity.
