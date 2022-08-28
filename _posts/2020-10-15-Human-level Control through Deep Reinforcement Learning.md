---
layout: post
tags: papers-i-read reinforcement-learning
title: Human level Control through Deep Reinforcement Learning
---

[Link to Paper](https://www.nature.com/articles/nature14236?wm=book_wap_0005)

Reinforcement learning is being used to master several difficult tasks. However, these agents struggle in deriving representations from high-dimensional sensory inputs. On the other hand, humans ace at these tasks through a “harmonious combination of reinforcement learning and hierarchical sensory processing system”.

This work spans the disjoint between high dimensional inputs and actions by combining machine learning with biologically inspired techniques to create RL agents capable of mastering diverse complex tasks. A novel deep Q-network agent incorporating reinforcement learning with ANN, and replay algorithm is built. 

The deep convolutional NN is used to approximate the action-value(Q) function. Due to this nonlinear function, the RL algorithm can diverge. To stabilize this, the observations are randomized to remove correlations (though experience replay) and correlation in the trager are removed by iteratively updating Q periodically. Hence, the target’s Q-learning updates are generated separately by the network.

The Q-network agent draws insight from experience replay, based on the neurobiological understanding that perceptual learning in the primate visual cortex is influenced by reward signals. Hence the agents experiences are stored at each time step.

Receiving only the pixels and game score as inputs, the agent outperforms human experts, while surpassing all current benchmarks on 49 Atari 2600 games. To be able to use the same learning rate across multiple games, the reward structure is modified to limit the error derivative. All positive, negative and zero rewards were clipped at 1, 21 and left unchanged respectively.

It is interesting to note that this is achieved by using the same algorithm, network architecture and hyperparameters across all games. The agent is able to learn representations and generalise it to varied other environments and control policies, than on which it was trained.It is hence capable of learning an array of complex tasks with the same parameter set and system.

