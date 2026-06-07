# $\beta$-TCVAE (Total Correlation VAE)

$\beta$-TCVAE provides a way to achieve disentanglement by decomposing the evidence lower bound (ELBO) and specifically targeting the Total Correlation term without an auxiliary discriminator.

## 🏗️ Architecture Diagram
*(Diagram available in the research paper below)*
> [View Diagram in Paper (Figure 1)](https://arxiv.org/pdf/1802.04942.pdf#page=4)

## 🔑 Key Features
- **ELBO Decomposition:** Mathematically breaks down the standard KL term into three components: Index-Code MI, Total Correlation, and Dimension-wise KL.
- **State-of-the-Art Disentanglement:** Isolates the TC term directly, often outperforming $\beta$-VAE and FactorVAE.
- **No Extra Hyperparameters:** Does not require the discriminator training complexity of FactorVAE.

## 📝 Research Paper
*   [Isolating Sources of Disentanglement in Variational Autoencoders (Chen et al., 2018)](https://arxiv.org/abs/1802.04942)

---
[⬅️ Back to README](../README.md)
