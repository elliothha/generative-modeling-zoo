# Generative Modeling Zoo
![GitHub last commit](https://img.shields.io/github/last-commit/elliothha/generative-modeling-zoo)

*[3/16/24 Update] Updated Gaussian-Bernoulli RBM to Bernoulli-Bernoulli RBM for MNIST generation. Uploaded old DCGAN notebook to GAN repo. Uploaded Normalizing Flow models (currently doesn't converge)*

*[3/15/24 Update] Updated MCMC Sampling Algos repo to have random-walk MH and MALA. Uploaded VAE model for MNIST generation*

---

This repo contains links to all of my Pytorch implementations for the various architectures and models in the generative modeling zoo. All implementations are intended purely for educational/academic purposes with sources cited.

Descriptions for the two main model categories paraphrased from Yang Song's [blogpost](https://yang-song.net/blog/2021/score/) on generative modeling.

by **Elliot H Ha**. Duke University

[elliothha.tech](https://elliothha.tech/) | [elliot.ha@duke.edu](mailto:elliot.ha@duke.edu)

---

## Architectures / Models
### Implicit generative models
Implicit generative models have the probability distribution implicitly represented by a model of its sampling process.
- Adversarial models
   - [Generative Adversarial Networks (GANs)](https://github.com/elliothha/generative-adversarial-networks)
      - Deep Convolutional GAN (DCGAN)
- Score-based models
   - Noise-Conditional Score Networks (NCSNs)
   - Score Networks w/ Stochastic Differential Equations (SDEs)
 
### Likelihood-based models
Likelihood-based models directly learn the distribution’s probability density (or mass) function via (approximate) maximum likelihood estimation.
 - Attention-based models
    - [Transformers](https://github.com/elliothha/transformers)
 - Autoencoder-based models
    - [Variational Autoencoders (VAEs)](https://github.com/elliothha/variational-autoencoders)
    - Masked Autoencoder for Distribution Estimation (MADE)
 - Energy-based models
    - [Restricted Boltzmann Machines (RBMs)](https://github.com/elliothha/restricted-boltzmann-machines)
 - Flow-based models
   - [Normalizing Flows (Autoregressive + Coupling)](https://github.com/elliothha/normalizing-flows)
      - Real NVP, NICE, MAF, IAF, GLOW
- Tree-based models
   - Chow-Liu Algorithm


## Sampling Algorithms

- [MCMC Sampling Algorithms](https://github.com/elliothha/mcmc-sampling-algos)
    - Random-walk Metropolis-Hastings Algorithm (+ Metropolis Algo)
    - Metropolis Adjusted Langevin Algorithm (MALA)
    - An example of Gibbs Sampling can be found in the [RBM repo](https://github.com/elliothha/restricted-boltzmann-machines/tree/main)
- (Annealed) Langevin Dynamics Sampling will be found in the NCSN repo if I ever finish it

---

## TODO
- [x] [3/15/24] ~~MCMC Sampling Algos for MH, MALA~~
- [x] [3/15/24] ~~VAE implementation for MNIST~~
- [x] [3/16/24] ~~Bernoulli-Bernoulli RBMs w/ Persistent Contrastive Divergence & Gibbs Sampling~~ 
- [x] [3/16/24] ~~Found my old notebook for DCGANs thank GOD~~
- [ ] Consolidate current notebook for the mess that is Norm Flows
- [ ] Adapt current Transformer architecture for autoregressive generation (NLP type stuff)
### Unfinished Implementations
- [ ] NCSNs w/ Annealed Langevin Dynamics Sampling, idk if I'll finish this honestly I strongly dislike score models
- [ ] "Attention Is All You Need" Transformer for NLP
- [ ] Chow-Liu Algo for decision trees, this one's super cool I'm probably going to finish this next
- [ ] Would be really cool to finish implementations for WaveNet/Parallel WaveNet for audio gen
