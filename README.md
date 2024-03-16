# Generative Modeling Zoo
![GitHub last commit](https://img.shields.io/github/last-commit/elliothha/generative-modeling-zoo)

*[3/16/24 Update] Updated Gaussian-Bernoulli RBM to Bernoulli-Bernoulli RBM for MNIST generation.*

*[3/15/24 Update] Updated MCMC Sampling Algos repo to have random-walk MH and MALA. Uploaded VAE model for MNIST generation*

This repo contains links to all of my Pytorch implementations for the various architectures and models in the generative modeling zoo. All implementations are intended purely for educational/academic purposes with sources cited.

Descriptions for the two main model categories paraphrased from Yang Song's [blogpost](https://yang-song.net/blog/2021/score/) on generative modeling.

by **Elliot H Ha**. Duke University

[elliothha.tech](https://elliothha.tech/) | [elliot.ha@duke.edu](mailto:elliot.ha@duke.edu)

---

## Architectures / Models
### Implicit generative models
Implicit generative models have the probability distribution implicitly represented by a model of its sampling process.
- GANs
   - [Generative Adversarial Networks (GANs)](https://github.com/elliothha/generative-adversarial-networks)
- Score-based models
   - [Noise-Conditional Score Networks (NCSNs)](https://github.com/elliothha/noise-conditional-score-networks)
 
### Likelihood-based models
Likelihood-based models directly learn the distribution’s probability density (or mass) function via (approximate) maximum likelihood estimation.
 - Autoregressive models
   - [Transformers](https://github.com/elliothha/transformers)
       - Attention Is All You Need
 - Energy-based models
    - [Restricted Boltzmann Machines (RBMs)](https://github.com/elliothha/restricted-boltzmann-machines)
 - Flow-based models
   - [Normalizing Flows (Autoregressive + Coupling)](https://github.com/elliothha/normalizing-flows)
      - RealNVP, NICE, MAF, IAF, GLOW
- Tree-based models
   - Chow-Liu Algorithm
- VAEs
  - [Variational Autoencoders (VAEs)](https://github.com/elliothha/variational-autoencoders)


## Sampling Algorithms

- [MCMC Sampling Algorithms](https://github.com/elliothha/mcmc-sampling-algos)
    - Random-walk Metropolis-Hastings Algorithm (+ Metropolis Algo)
    - Metropolis Adjusted Langevin Algorithm (MALA)

---

## TODO
- [x] [3/15/24] ~~MCMC Sampling Algos~~
- [x] [3/15/24] ~~VAEs~~
- [ ] Find my old notebooks for GANs, RBMs
- [ ] Consolidate current notebooks for Norm Flows, Transformers
### Unfinished Implementations
- [ ] NCSNs w/ Annealed Langevin Dynamics Sampling
- [ ] Transformer for NLP
- [ ] Chow-Liu Algo
