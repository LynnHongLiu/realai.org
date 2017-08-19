---
permalink: /architecture-search/
---
# Architecture Search

Manually designing deep neural networks requires a lot of expert knowledge, and is very time-consuming. Many techniques have been proposed to automate this process. [Brock et al. (2017)](https://arxiv.org/abs/1708.05344) propose the SMASH method for architecture search. It learns an auxiliary HyperNet ([Ha et al., 2016](https://arxiv.org/abs/1609.09106)) to generate a model’s weights based on its architecture, and uses the performance of these generated models on the validation error to approximate their performance when using normally trained weights. By using the generated weights, they can effectively search over a wide range of architectures with much less computation. They also develop a mechanism based on memory read-writes to encode architectures for the HyperNet. SMASH is validated on CIFAR-10 and CIFAR-100, STL-10, ModelNet10, and Imagenet32x32, achieving competitive performance.

[Negrinho & Gordon (2017)](https://arxiv.org/abs/1704.08792) used an extensible and modular language to describe expressive spaces of model parameters, which then can be searched using Monte Carlo tree search and sequential model-based optimization.

## Evolutionary Algorithms

While gradient methods are very effective in learning the weights of neural connections, evolutionary algorithms aim to address the issue of what connect to what in the first place ([Stanley, 2017](https://www.oreilly.com/ideas/neuroevolution-a-different-kind-of-deep-learning)).

### References

* 2017 July 13, Kenneth O. Stanley. [Neuroevolution: A different kind of deep learning](https://www.oreilly.com/ideas/neuroevolution-a-different-kind-of-deep-learning). *O'Reilly*.
* 2017 March 3, Esteban Real, Sherry Moore, Andrew Selle, Saurabh Saxena, Yutaka Leon Suematsu, Quoc Le, and Alex Kurakin. [Large-Scale Evolution of Image Classifiers](https://arxiv.org/abs/1703.01041). *arXiv:1703.01041*.
* 2017 March 1, Risto Miikkulainen, Jason Liang, Elliot Meyerson, Aditya Rawal, Dan Fink, Olivier Francon, Bala Raju, Arshak Navruzyan, Nigel Duffy, and Babak Hodjat. [Evolving Deep Neural Networks](https://arxiv.org/abs/1703.00548). *arXiv:1703.00548*.
* 2016 June 8, Chrisantha Fernando, Dylan Banarse, Malcolm Reynolds, Frederic Besse, David Pfau, Max Jaderberg, Marc Lanctot, and Daan Wierstra. [Convolution by Evolution: Differentiable Pattern Producing Networks](https://arxiv.org/abs/1606.02580). *arXiv:1606.02580*.

## Reinforcement Learning

[Zoph & Le (2016)](https://arxiv.org/abs/1611.01578) use reinforcment learning to train a recurrent network that generates descriptions of neural networks to minimize validation error, then found convolutional and LTSM architectures that performed competitively in CIFAR-10 and Penn Treebank datasets, respectively. Using this approach, [Zoph et al. (2017)](https://arxiv.org/abs/1707.07012) learn a convolutional cell on the CIFAR-10 dataset that can be transferred to the ImageNet dataset. By stacking together more of this cell, they achieve better top-1 accuracy than the best human-invented architectures with less computation.

[Cai et al. (2017)](https://arxiv.org/abs/1707.04873) train a reinforcement learning agent to grow the depth or layer width of a neural network, allowing previously learned weights to be reused.

## References

* 2017 August 18, Andrew Brock, Theodore Lim, J. M. Ritchie, and Nick Weston. [SMASH: One-Shot Model Architecture Search through HyperNetworks](https://arxiv.org/abs/1708.05344). *arXiv:1708.05344*. [code](https://github.com/ajbrock/SMASH). [video](https://www.youtube.com/watch?v=79tmPL9AL48).
* 2017 July 21, Barret Zoph, Vijay Vasudevan, Jonathon Shlens, and Quoc V. Le. [Learning Transferable Architectures for Scalable Image Recognition](https://arxiv.org/abs/1707.07012). *arXiv:1707.07012*.
* 2017 July 16, Han Cai, Tianyao Chen, Weinan Zhang, Yong Yu, and Jun Wang. [Reinforcement Learning for Architecture Search by Network Transformation](https://arxiv.org/abs/1707.04873). *arXiv:1707.04873*.
* 2017 April 28, Renato Negrinho and Geoff Gordon. [DeepArchitect: Automatically Designing and Training Deep Architectures](https://arxiv.org/abs/1704.08792). *arXiv:1704.08792*.
* 2016 December 1, David Ha, Andrew Dai, and Quoc V. Le. [HyperNetworks](https://arxiv.org/abs/1609.09106). *arXiv:1609.09106*.
* 2016 November 7, Bowen Baker, Otkrist Gupta, Nikhil Naik, and Ramesh Raskar. [Designing Neural Network Architectures using Reinforcement Learning](https://arxiv.org/abs/1611.02167). *arXiv:1611.02167*.
* 2016 November 5, Barret Zoph and Quoc V. Le. [Neural Architecture Search with Reinforcement Learning](https://arxiv.org/abs/1611.01578). *arXiv:1611.01578*.
