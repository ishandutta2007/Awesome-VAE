# $\beta$-VAE (Beta-VAE)

$\beta$-VAE is a modification of the standard VAE framework that introduces a hyperparameter $\beta$ to control the emphasis on learning independent (disentangled) latent factors.

## 🏗️ Architecture Diagram
![Beta-VAE Block Scheme](https://www.researchgate.net/profile/Leonardo-Crespi/publication/354123456/figure/fig1/AS:11431281234567168@1712640000000/A-block-scheme-of-the-beta-VAE.png)

## 🔑 Key Features
- **Disentanglement:** By setting $\beta > 1$, the model is forced to prioritize the KL-divergence term, leading to a more compact and independent latent space.
- **Interpretable Features:** Different dimensions often correspond to human-interpretable traits like object rotation, color, or scale.
- **Information Bottleneck:** Effectively acts as a controllable information bottleneck.

## 📝 Research Paper
*   [$\beta$-VAE: Learning Basic Visual Concepts with a Constrained Variational Framework (Higgins et al., 2017)](https://openreview.net/forum?id=Sy2fzU9gl)

---
[⬅️ Back to README](../README.md)
