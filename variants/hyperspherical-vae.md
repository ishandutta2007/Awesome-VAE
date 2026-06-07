# Hyperspherical VAE ($\mathcal{S}$-VAE)

The Hyperspherical VAE maps latent variables onto the surface of a hypersphere ($\mathcal{S}^n$) rather than a flat Euclidean space, using the von Mises-Fisher (vMF) distribution.

## 🏗️ Architecture Diagram
![Hyperspherical VAE Concept](https://raw.githubusercontent.com/nicola-decao/s-vae/master/toy1.png)

## 🔑 Key Features
- **Non-Euclidean Latent Space:** Ideal for data with a directional or cyclical nature.
- **Uniform Prior:** The hyperspherical surface naturally provides a uniform prior, avoiding the "center-seeking" bias of Gaussian VAEs.
- **vMF Distribution:** Replaces the standard Gaussian with the von Mises-Fisher distribution for sampling on the sphere.

## 📝 Research Paper
*   [Hyperspherical Variational Auto-Encoders (Davidson et al., 2018)](https://arxiv.org/abs/1804.00891)

---
[⬅️ Back to README](../README.md)
