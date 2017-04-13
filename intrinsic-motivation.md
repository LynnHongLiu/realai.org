---
permalink: /intrinsic-motivation/
---
# Intrinsic Motivation

The rewards reinforcement learning agents receive are commonly interpreted as signals from the achievement of desired outcomes, such as completion of tasks or high scores in games. But in most realistic settings such rewards are sparse and it's increasingly important for agents to rely on *internal* rewards to learn useful skills. These rewards should not be designed based on details of the *external* problems the agents learn to solve.

[Florensa et al. (2017)](https://arxiv.org/abs/1704.03012) designed a single proxy reward that encodes the prior about useful high level bahaviors, then combined Stochastic Neural Networks with mutual information to encourage diversity of skills.

There are many ([Oudeyer & Kaplan, 2008](http://www.lucs.lu.se/LUCS/139/oudeyer.pdf)) intrinsic motivations, some commonly used ones include:

* Empowerment
* [Exploration](http://realai.org/exploration/)
* Mutual Information
* [Prediction](http://realai.org/predictive-learning/)

## References

* 2017 April 10, Carlos Florensa, Yan Duan, and Pieter Abbeel. [Stochastic Neural Networks for Hierarchical Reinforcement Learning](https://arxiv.org/abs/1704.03012). *arXiv:1704.03012*.
* 2008 July 30, Pierre-Yves Oudeyer and Frederic Kaplan. [How can we define intrinsic motivation?](http://www.lucs.lu.se/LUCS/139/oudeyer.pdf). *Proceedings of the Eighth International Conference on Epigenetic Robotics: Modeling Cognitive Development in Robotic Systems*, 93-101.