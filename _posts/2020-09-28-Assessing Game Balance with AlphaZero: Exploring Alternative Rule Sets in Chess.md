---
layout: post
tags: papers-i-read deep-learning AlphaZero
title: Assessing Game Balance with AlphaZero- Exploring Alternative Rule Sets in Chess
---

[Link to Paper](https://arxiv.org/pdf/2009.04374.pdf)

> Turing (1953) asked, “Could one make a machine to play chess,
and to improve its play, game by game, profiting from its
experience?”

This chess paper reminds how beautiful a game can be. The paper covers too much for me to be able to wrap in this article. Regardless.

The paper utilises AlphaZero for game balance assessment of new chess variants. By learning each variant, the potential of these chess adaptations is determined. The paper answers how fair a variant of chess is? What happens when even a small rule is changed?

Nine alterations to the modern ches are explored in the paper, including wild variants like self-capture and pawn sideways. As no prior gaming knowledge is required for AlphaZero to train, different rules are rapidly explored through both quantitative(expected scores, draw rates, effects of special moves, etc) and qualitative comparisons.

Few points from the paper -
- Alpha Zero was surprisingly accurate in computing material value of pieces proportionate to pawn. It computes 1-3.05-3.33-5.63-9.5! In classical chess it is 1-3-3.5-5-9!
- To encourage exploration by AlphaZero during training, a small amount of noise is injected along with the prior move probabilities.
- To learn the chess piece values, a linear model is trained over sampled states of games with a mean-square-error loss and tanh activation. Simple and straight formulation!
- Several chess variants- Torpedo, Semi-torpedo, No-castling chess and Stalemate, turn out to be more decisive than classical chess.
- In the self-capture games, AlphaZero captures its own queen when in an already winning position!

The paper is a very interesting read! Chess is theoretically a drawn dame, testing alternate hypotheses and actually simulating decades of human play with them within a few hours, something that would have taken a long period of time and a large number of human players, is super neat!

Maybe this can be the new standard to design new games in the future!
