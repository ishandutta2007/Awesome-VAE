# $\beta$-TCVAE (Total Correlation VAE)

$\beta$-TCVAE provides a way to achieve disentanglement by decomposing the evidence lower bound (ELBO) and specifically targeting the Total Correlation term without an auxiliary discriminator.

## 🏗️ Architecture Diagram
*(Diagram to be added)*

## 🔑 Key Features
- **ELBO Decomposition:** Mathematically breaks down the standard KL term into three components: Index-Code MI, Total Correlation, and Dimension-wise KL.
- **State-of-the-Art Disentanglement:** Isolates the TC term directly, often outperforming $\beta$-VAE and FactorVAE.
- **No Extra Hyperparameters:** Does not require the discriminator training complexity of FactorVAE.

## 📝 Research Paper
*   [Isolating Sources of Disentanglement in Variational Autoencoders (Chen et al., 2018)](https://arxiv.org/abs/1802.04942)

---
[⬅️ Back to README](../README.md)
