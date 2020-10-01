---
layout: post
categories: Papers-I-Read
title: Understanding Deep Learning requires Rethinking Generalization
tags: [Papers-I-Read, Deep Learning, Generalization, ICLR]
---

[Link to Paper](https://arxiv.org/abs/1611.03530)

The paper questions why some models generalize better than others. Which basically at heart means why neural networks work the way they do? Through experimentation, it is shown that traditional statistical approaches fail to explain generalization in neural networks and conclude that a precise formal measure to explain this is yet to exist. The authors discuss model capacity and find that even though regularisation improves generalization performance, it is still possible to get good generalization with no regularization.

The paper soundly questioned many notions that aren’t talked about much and are significant enough actually to be. Following are my major takeaways and best bits from the paper - 

- I think it was intriguing that the hyperparameters did not have to be changed for the NN to fit random labels, inferring that hyperparameters might depend more on the network architecture than the data itself. 

- The subplot of the learning curves on CIFAR-10 is what grabbed my attention the most. The NN achieves zero training error on all permutation of settings with varying converging speeds. The data with the correct labels and the shuffled pixels converges fast, which is obvious. Interestingly, random labels converged the slowest, which I thought would happen to the gaussian distributed data. 

- Through the experiments, it can be gathered that explicit regularisation can be seen more like a tuning parameter for generalization as it’s absence does not imply bad generalization error. Another fascinating takeaway is that a certain amount of regularisation is picked up just by grturadient descent.

The authors argue that models likely do make use of massive memorization to perform well. As they have the capacity to fit noise, it is still unclear to me as to why generalized results are produced on real data. Maybe, we do need to rethink generalization.

Concluding, neural networks still seem mysterious. It looks like model architectures have been built such that they work well on images rather than the natural(actual) meaning of those images.
