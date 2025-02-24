# One Loss for All: Deep Hashing with a Single Cosine Similarity based Learning Objective

## Abstract

A deep hashing model typically has two main learning objectives:
to make the learned binary hash codes discriminative and to minimize a quantization error.
With further constraints such as bit balance and code orthogonality,
it is not uncommon for existing models to employ a large number (>4) of losses.
This leads to difficulties in model training and subsequently impedes their effectiveness.
In this work, we propose a novel deep hashing model with only a single learning objective.
Specifically, we show that maximizing the cosine similarity between the continuous codes
and their corresponding binary orthogonal codes can ensure both hash code discriminativeness
and quantization error minimization. Further, with this learning objective, code balancing
can be achieved by simply using a Batch Normalization (BN) layer and multi-label classification
is also straightforward with label smoothing. The result is an one-loss deep hashing model that
removes all the hassles of tuning the weights of various losses. Importantly, extensive experiments
show that our model is highly effective, outperforming the state-of-the-art multi-loss hashing models
on three large-scale instance retrieval benchmarks, often by significant margins.

## Code and Paper

[arXiv](https://arxiv.org/abs/2109.14449)

<a href="suppmat.pdf">Supplementary Material</a>

[Github](https://github.com/kamwoh/orthohash)