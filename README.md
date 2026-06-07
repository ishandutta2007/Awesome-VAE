# 🚀 Awesome-VAE: A Comprehensive Guide to Variational Autoencoder Variants

![GitHub stars](https://img.shields.io/github/stars/ishandutta2007/Awesome-VAE?style=flat-square)
![GitHub forks](https://img.shields.io/github/forks/ishandutta2007/Awesome-VAE?style=flat-square)
![GitHub repo size](https://img.shields.io/github/repo-size/ishandutta2007/Awesome-VAE?style=flat-square)
![GitHub issues](https://img.shields.io/github/issues/ishandutta2007/Awesome-VAE?style=flat-square)
![GitHub license](https://img.shields.io/github/license/ishandutta2007/Awesome-VAE?style=flat-square)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)

A curated, high-quality collection of **Variational Autoencoder (VAE)** research, architectures, and implementations. This repository maps out the evolution of VAE models in **machine learning**, **deep learning**, and **generative AI**—from standard continuous models to modern discrete, disentangled, and hierarchical variants like **VQ-VAE**, **Beta-VAE**, and **NVAE**.

---

## 📌 Table of Contents
- [1. 🧩 Discrete & Token-Based VAEs](#1--discrete--token-based-vaes)
- [2. ✨ Disentangled VAEs](#2--disentangled-vaes)
- [3. 🏗️ Structural & Hierarchical VAEs](#3--structural--hierarchical-vaes)
- [4. 🌀 Advanced Geometric & Flow VAEs](#4--advanced-geometric--flow-vaes)
- [📊 Quick Comparison Matrix](#-quick-comparison-matrix)
- [🤝 Contributing](#-contributing)

---

## 1. 🧩 Discrete & Token-Based VAEs
These variants replace continuous probability distributions with discrete tokens, making them highly effective for data compression and serving as components for foundational AI models.

| Variant | Key Mechanism | Year | Research Paper |
| :--- | :--- | :--- | :--- |
| **[VQ-VAE](variants/vq-vae.md)** | Discrete codebook mapping to prevent blurriness | 2017 | [DeepMind](https://arxiv.org/abs/1711.00937) |
| **[VQ-VAE-2](variants/vq-vae-2.md)** | Multi-scale hierarchical discrete codebooks | 2019 | [DeepMind](https://arxiv.org/abs/1906.00446) |
| **[Gumbel-Softmax VAE](variants/gumbel-softmax-vae.md)** | Differentiable categorical relaxation trick | 2016 | [Google Brain](https://arxiv.org/abs/1611.01144) |

---

## 2. ✨ Disentangled VAEs
These models constrain individual dimensions of the latent space to represent distinct, independent physical features (e.g., face angle, lighting, or hair color).

| Variant | Disentanglement Strategy | Year | Research Paper |
| :--- | :--- | :--- | :--- |
| **[$\beta$-VAE](variants/beta-vae.md)** | Scaled KL-divergence penalty hyperparameter | 2017 | [DeepMind](https://openreview.net/forum?id=Sy2fzU9gl) |
| **[FactorVAE](variants/factor-vae.md)** | Total Correlation penalty via discriminator | 2018 | [DeepMind](https://arxiv.org/abs/1802.05983) |
| **[$\beta$-TCVAE](variants/beta-tcvae.md)** | ELBO decomposition targeting Total Correlation | 2018 | [MS Research](https://arxiv.org/abs/1802.04942) |

---

## 3. 🏗️ Structural & Hierarchical VAEs
These variants modify the routing and depth of the latent space to capture complex, multi-layered data dependencies.

| Variant | Architecture Modification | Year | Research Paper |
| :--- | :--- | :--- | :--- |
| **[Conditional VAE (CVAE)](variants/cvae.md)** | Latent conditioning on labels/metadata | 2015 | [NIPS 2015](https://proceedings.neurips.cc/paper/2015/hash/8d55a249e6baa5c06772297520da2051-Abstract.html) |
| **[Hierarchical VAE (HAE)](variants/hae.md)** | Layered latent variable stacking (Ladder) | 2016 | [NIPS 2016](https://arxiv.org/abs/1602.02282) |
| **[Nouveau VAE (NVAE)](variants/nvae.md)** | Deep residual hierarchical cells optimization | 2020 | [NVIDIA](https://arxiv.org/abs/2007.03898) |

---

## 4. 🌀 Advanced Geometric & Flow VAEs
These models replace traditional standard Gaussian distributions with more complex mathematical spaces or coordinate systems.

| Variant | Geometric/Probabilistic Space | Year | Research Paper |
| :--- | :--- | :--- | :--- |
| **[Normalizing Flow VAE](variants/flow-vae.md)** | Invertible transformation sequences (flows) | 2015 | [ICML 2015](https://arxiv.org/abs/1505.05770) |
| **[Hyperspherical VAE](variants/hyperspherical-vae.md)** | Latent mapping to von Mises-Fisher surface | 2018 | [UvA](https://arxiv.org/abs/1804.00891) |
| **[Graph VAE (GVAE)](variants/graph-vae.md)** | Non-Euclidean data/adjacency reconstruction | 2016 | [NIPS 2016](https://arxiv.org/abs/1611.07308) |

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
### 📜 License
This project is licensed under the [MIT License](LICENSE).

<!-- Keywords: Variational Autoencoder, VAE variants, Machine Learning, Deep Learning, Generative Models, Neural Networks, AI architectures, VQ-VAE, Beta-VAE, CVAE, NVAE, PyTorch, TensorFlow, Latent Space, Disentanglement, Hierarchical VAE, Normalizing Flows -->
