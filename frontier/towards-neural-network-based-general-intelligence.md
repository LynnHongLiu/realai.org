---
permalink: /frontier/towards-neural-network-based-general-intelligence.html
---
# Towards Neural Network-Based General Intelligence

*Below is a list of obstacles we believe are on the paths from today's technologies to general AI. As our understanding improves, this list will be revised from time to time. When this page develops into a coherent piece of scholarly value, we plan to publish it on arXiv. Comments should be directed to [Jonathan Yan](mailto:jyan@realai.org).*

## Introduction 

The problems listed below are interrelated, the solution of one part of a problem is often closely related to the solution of one part of another problem. AGI may be attainable after satisfactory solutions of only a few problems.

## 1. Learning Architecture

It is not yet clear how a general AI system's internal states should change according to inputs. At present, the optimization of an objective function motivates most of the standard update rules, e.g. SGD, momentum, Adagrad, Adadelta, RMSprop, and Adam.

There may be new update rules that are more directly linked to inputs. Network weights and topology can also change over time, sometimes according to outputs from other networks.

## 2. Unsupervised Learning

In the more likely case that update rules are motivated by optimization, the ability of unsupervised learning requires the objectives of optimization to be relatively stable and likely intrinsic.

### 2.1 Intrinsic Motivations

Here we include the type of update rules that are driven by the optimization of physics-inspired quantities such as free energy.

#### 2.1.1 Predictive Learning

The system learns to predict future inputs. This is likely harder than the study of *generative models* which only need to generate data without making extra moves through time.

#### 2.1.2 Exploration / Curiosity

The system prefers novel states.

## 3. Continual Learning

A general AI system can learn new tasks while largely retaining old knowledge.

### 3.1 Cumulative Learning

Training and testing phases should not be completely separate and can happen concurrently. 

## 4. Few Shot Learning

The system can easily generalize. Its encoded knowledge and continual learning ability allow it to learn new behaviors from much fewer data than today's narrow AI systems.

## 5. Hierarchical Learning

The ability to learn hierarchical structures in the data and use them for abstract planning and reasoning, sometimes in long time horizon. Hierarchies in network architeture are likely necessary.

### 5.1 Concept Learning

This can be seen as a special case where one level of hierarchy, from data to concept, needs to be solved.

## 6. Neural Interface and Modules

* The architecture needs to be independent enough to allow unlocked learning, so that modules can learn autonomously while communicating with other modules via cleverly designed interface;
* Multi-agent learning where each agent is considered a module and their means of communication the interface; and
* Stable input and output interfaces for interactions with the environment.

## 7. Basic Cognitive Functions

### 7.1 Memory

Memory can be a very useful component of the learning architecture and is often times not in the form neural networks, which are not particularly good at recording data.

#### 7.1.1 Episodic and long-term memory

#### 7.1.2 Temporary memory that facilitates learning e.g. used for experience replay

### 7.2 Attention

Selectively attend to the part of data that are important for the current context in which the system is operating.

### 7.3 Reasoning

The ability to reason in abstract terms is one way of hierarchical thinking.

## 8. Language Grounding

The system's understanding of language should be grounded to its representation of common sense knowledge, not merely finding patterns in texts. Language can be considered as the interface between neural network agents who need to communicate.

## 9. World Model

The learning system should contain a vast amount of knowledge that forms the basis of "common sense", which can be the result of continual learning.
