---
layout: post
categories: Papers-I-Read
title: Unsupervised Translation of Programming Languages
tags: [Papers-I-Read, Transcompiler, Unsupervised Learning]
---

[Link to Paper](https://arxiv.org/abs/2006.03511)

The paper introduces a novel unsupervised neural transcompiler, by purely using monolingual open source code from public Github repositories. The transcompiler is capable of converting code between C++, Java and Python programs, outperforming existing benchmarks. 

Majority of existing transcompilers are rule-based and have several disadvantages - tedious to write handcrafted rules, requires expertise in both source and target programming languages and issues with inferring variables from a dynamically to statically typed language. Other supervised approaches fall short due to the limited availability of parallel data. Hence, being able to do unsupervised machine translation discards all this.

To achieve the transcompiler, a single transcoder model is trained for all programming languages using a seq2seq model with attention, and an encoder-decoder(transformer) architecture. The three principles of machine translation are used - 

**Initialisaztion**. The model is initialised with cross-lingual words (anchor points - for, while, if) to map the same instructions to the same representation. For creating these representations, random words of an input code are masked and then predicted, at each iteration by the cross-lingual language(XLM) model.
 
**Language modelling**. The encoder and the decoder are initialised with the pretrained XLM model. The decoder is trained with a denoising auto-encoding(DAE) objective so that it always generates valid sequences even with noisy input, making the encoder more robust. The first token of the input specifies the programming language. Hence, one can decode in python and encode in java.

**Back translation**. Deriving from supervised machine translation, this is effectively used to improve model performance. It basically allows the model to itself generate data to train on by using a target-to-source technique.

The transcoder model is evaluated with 852 parallel functions and unit tests for each. For validation and test sets, parallel functions from GeeksforGeeks were taken. It is noteworthy that a new metric, “computational accuracy”(evaluates if the same output is given on the same inputs) was used to score the model rather than the lacking BLEU and reference match scoring.
