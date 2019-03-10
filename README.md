# IPNN-pytorch
**A pytorch implementation of "[Intriguing properties of neural networks](https://arxiv.org/abs/1312.6199)"**

## Summary
1. The natural basis is not better than a random basis for inspecting the properties of latent vectors.
 - there are serveral directions which have the semantic meaning not only individual units.
2. We can generate images(_adversarial examples_) with small perturbations to fooling neural network models.
3. Weight Decay or Regularization couldn't help model to defend adversarial examples.
4. One adversarial example for a specific model is possible to deceive other models.
5. According to spectral analysis of unstability, the deeper models, the more stupid.

## Requirements
* python==3.6   
* numpy==1.14.2   
* pytorch==1.0.0   

## Limitations of this code
In the paper, they use L-BFGS to solve equation with constraints.
However, in this code, backpropagation method is used instead of L-BFGS.
