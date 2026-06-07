# FactorVAE

FactorVAE is designed to achieve better disentanglement than $\beta$-VAE by directly penalizing the Total Correlation (TC) of the latent distribution.

## 🏗️ Architecture Diagram
![FactorVAE Architecture](https://www.researchgate.net/profile/Santiago-Jimenez/publication/341234567/figure/fig1/AS:11431281234567168@1712640000000/Architecture-of-the-FactorVAE.png)

## 🔑 Key Features
- **Total Correlation Penalty:** Adds a term to the loss function that minimizes the dependency between latent dimensions.
- **Adversarial Training:** Uses a discriminator network to estimate the Total Correlation.
- **Improved Reconstruction:** Often achieves better disentanglement than $\beta$-VAE without sacrificing as much reconstruction quality.

## 📝 Research Paper
*   [Disentangling by Factorising (Kim & Mnih, 2018)](https://arxiv.org/abs/1802.05983)

---
[⬅️ Back to README](../README.md)
