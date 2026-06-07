# Awesome-VAE
## Comprehensive Guide to Variational Autoencoder (VAE) Variants

[![License: MIT](https://shields.io)](https://opensource.org)
[![PRs Welcome](https://shields.io)](http://makeapullrequest.com)

A curated, structured overview of the major types of Variational Autoencoders (VAEs). This repository maps out the evolution of VAE architectures from standard continuous models to modern discrete, disentangled, and hierarchical variants.

---

## 📌 Table of Contents
- [1. Discrete & Token-Based VAEs](#1-discrete--token-based-vaes)
- [2. Disentangled VAEs](#2-disentangled-vaes)
- [3. Structural & Hierarchical VAEs](#3-structural--hierarchical-vaes)
- [4. Advanced Geometric & Flow VAEs](#4-advanced-geometric--flow-vaes)
- [📊 Quick Comparison Matrix](#-quick-comparison-matrix)
- [🤝 Contributing](#-contributing)

---

## 1. Discrete & Token-Based VAEs
These variants replace continuous probability distributions with discrete tokens, making them highly effective for data compression and serving as components for foundational AI models.

*   **VQ-VAE (Vector Quantized VAE):** Maps continuous latent vectors to the nearest discrete vector in a learned "codebook". This prevents blurriness and posterior collapse, forming the tokenization backbone for generative architectures like DALL-E.
*   **VQ-VAE-2:** A hierarchical upgrade to VQ-VAE that uses multi-scale codebooks (e.g., a top-level codebook for global shape and a bottom-level codebook for fine textures) to generate high-resolution data.
*   **Gumbel-Softmax VAE:** Utilizes the Gumbel-Softmax distribution trick to backpropagate gradients through discrete latent variables without a fixed codebook, allowing the neural network to make categorical choices natively.

---

## 2. Disentangled VAEs
These models constrain individual dimensions of the latent space to represent distinct, independent physical features (e.g., face angle, lighting, or hair color).

*   **$\beta$-VAE:** Introduces a hyperparameter ($\beta > 1$) to scale the Kullback-Leibler (KL) divergence loss. This prioritizes latent independence, trading off a small amount of reconstruction quality for highly interpretable features.
*   **FactorVAE:** Disentangles features more effectively than $\beta$-VAE by directly penalizing the *Total Correlation* of the latent distribution using an auxiliary discriminator network.
*   **$\beta$-TCVAE (Total Correlation VAE):** Achieves state-of-the-art disentanglement by mathematically breaking down the standard KL divergence equation, isolating the total correlation term without requiring an extra discriminator network.

---

## 3. Structural & Hierarchical VAEs
These variants modify the routing and depth of the latent space to capture complex, multi-layered data dependencies.

*   **Conditional VAE (CVAE):** Feeds a label or condition (e.g., a specific digit class or text prompt) into both the encoder and decoder. This allows users to direct the model to generate a specific class of output.
*   **Hierarchical VAE (HAE):** Stacks multiple latent layers sequentially. Lower layers capture coarse, global structures, while deeper layers capture fine, local details.
*   **Nouveau VAE (NVAE):** A highly optimized, deep hierarchical VAE that uses depth-wise separable convolutions and residual cells to generate high-resolution continuous images that rival early GANs.

---

## 4. Advanced Geometric & Flow VAEs
These models replace traditional standard Gaussian distributions with more complex mathematical spaces or coordinate systems.

*   **Normalizing Flow VAE:** Passes a simple standard Gaussian distribution through a series of invertible mathematical transformations (flows) to warp it into a highly complex, expressive probability shape.
*   **Hyperspherical (von Mises-Fisher) VAE:** Maps latent variables onto the surface of a hypersphere instead of a flat hyper-plane, which is ideal for directional data like earth mapping or molecular orientation.
*   **Graph VAE (GVAE):** Tailored to process non-Euclidean data by encoding and decoding node features and edge adjacency matrices. Commonly used for molecular generation and social network analysis.

---

## 📊 Quick Comparison Matrix


| VAE Variant | Core Latent Space Mechanism | Key Performance Metric / Objective | Primary Use Case |
| :--- | :--- | :--- | :--- |
| **Standard VAE** | Continuous Gaussian Mapping | Reconstructs data smoothly | Smooth interpolations, basic synthesis |
| **CVAE** | Condition/Label Injected Space | Targeted sample generation | Controlled generation (e.g., Text-to-Image) |
| **$\beta$-VAE** | Scaled KL Divergence Penalty | Maximizes feature isolation | Feature explanation and interpretability |
| **VQ-VAE** | Nearest-Neighbor Codebook | Discretizes space without information loss | Text, audio, and high-fidelity image tokens |
| **NVAE** | Deep Residual Hierarchical Layers | Optimizes high-res continuous outputs | Ultra-high-resolution continuous generation |
| **Flow VAE** | Invertible Geometric Flows | Increases density estimation accuracy | Complex, highly expressive distributions |

---

## 🤝 Contributing
Contributions are welcome! If you would like to add a new VAE variant, include PyTorch/TensorFlow implementations, or provide training tips:
1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/vae-variant`).
3. Commit your changes (`git commit -m 'Add descriptive VAE type'`).
4. Push to the branch (`git push origin feature/vae-variant`).
5. Open a Pull Request.


## 📈 Star History

<div align="center">
	<a href="https://www.star-history.com/?repos=ishandutta2007%2FAwesome-VAE&type=date&legend=bottom-right">
	 <picture>
	   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/chart?repos=ishandutta2007/Awesome-VAE&type=date&theme=dark&legend=bottom-right" />
	   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/chart?repos=ishandutta2007/Awesome-VAE&type=date&legend=bottom-right" />
	   <img alt="Star History Chart" src="https://api.star-history.com/chart?repos=ishandutta2007/Awesome-VAE&type=date&legend=bottom-right" />
	 </picture>
	</a>
</div>


---
License: [MIT](LICENSE)
