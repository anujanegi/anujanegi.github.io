---
layout: post
categories: Papers-I-Read
title: Natural Image Reconstruction from Brain Waves - a Novel Visual BCI System with Native Feedback
tags: [Papers-I-Read, Image Reconstruction, Brain Computer Interface, EEG]
---

[Link to Paper](https://www.biorxiv.org/content/10.1101/787101v3)

Utilizing non-invasive EEG recordings, the paper introduces a closed BCI system capable of reconstructing observed or imagined stimuli images from co-occurring brain parameters. The authors are successfully able to gather from the advantages of both synchronous and asynchronous BCI systems. They use the correlation between long-term evoked responses and mental states triggered by a particular simulation, along with native feedback, to develop this novel BCI paradigm.

The two main objectives of the research are to study the brain activity upon continuous visual stimuli and to then develop a model capable of mapping these EEG features to the stimuli and hence reconstruct the natural image back. 

To explore the first, the EEG signals of 17 healthy human subjects observing video clips of varied objects (from different categories) were recorded over two sessions. To avoid parasite ERPs, no clips were repeated and no montage transitions were included. 

To achieve the second objective, feature extraction was performed within the ICA matrix space, using artifact rejection, Fourier transforms for spectral feature extraction, and PCA for reduced dimensionality. These features were classified using LDA (linear discriminant analysis into categories. To guarantee that signals aren't biased to any class, the “Goldberg mechanism” category is chucked on the caution of containing parasite discriminative features due to eye movement. How cautious!

To establish the native neurofeedback, an image autoencoder (independent of any neurophysiological data) is used for the reconstruction of natural images. I like how the loss function uses distance, angle, and pixel loss for parameter tuning. Further, availing the fact that the experiment has continuous data, RNNs are used for the EEG feature mapping (translates EEF feature domain to image decoder space). 

While testing, a subject was also able to switch between the categories at his own will without even watching the actual video clips and was hence able to master imaginary switching within 10 minutes of training! The results obtained are impressive and make me even more excited about what is possible using BCI systems in the future. Taking inspiration from this, how can we head towards better brain-controlled technology?

The authors successfully show their hypothesis, “observing the visual stimuli of different categories trigger distinct brain states'' and that it is possible to vary the stimuli without affecting the inter-category separability. They achieve a closed-loop BCI system capable of real-time, mind-driven image reconstruction using EEG features. As there are no additional cognitive tasks associated, it makes it even suitable for those patients with cognitive disorders.

Food for the brain -  If we have these models trained on bigger datasets and, if someone who is trained and effectively able to master imaginary and precisely visualize images in their own mind - could we then visualize thoughts?

