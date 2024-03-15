# Generative Modeling Zoo

*[3/15/23 Update] Updated MCMC Sampling Algos repo to have random-walk MH and MALA*

This repo contains links to all of my Pytorch implementations for the various architectures and models in the generative modeling zoo. All implementations are intended purely for educational/academic purposes with sources cited.

[TODO]: Need to track down my old files for GANs, VAEs, and RBMs, and then also consolidate my current notebooks for Norm Flows and Transformers into the repos :( Will do sometime later this week hopefully when I have time. Also need to try implementing NCSNs based off the paper

by **Elliot H Ha**. Duke University

---

## Architectures / Models

### Implicit generative models
- GANs
   - [Generative Adversarial Networks (GANs)](https://github.com/elliothha/generative-adversarial-networks)
- Score-based models
   - [Noise-Conditional Score Networks (NCSNs)](https://github.com/elliothha/noise-conditional-score-networks)
 
### Likelihood-based models
 - Autoregressive models
   - [Transformers](https://github.com/elliothha/transformers)
       - Attention Is All You Need
 - Energy-based models
    - [Restricted Boltzmann Machines (RBMs)](https://github.com/elliothha/restricted-boltzmann-machines)
 - Flow-based models
   - [Normalizing Flows (Autoregressive + Coupling)](https://github.com/elliothha/normalizing-flows)
      - RealNVP, NICE, MAF, IAF, GLOW
- VAEs
  - [Variational Autoencoders (VAEs)](https://github.com/elliothha/variational-autoencoders)


## Markov Chain Monte Carlo (MCMC) Sampling Algorithms

- [MCMC Sampling Algorithms](https://github.com/elliothha/mcmc-sampling-algos)
    - Random-walk Metropolis-Hastings Algorithm (+ Metropolis Algo)
    - Metropolis Adjusted Langevin Algorithm (MALA)
