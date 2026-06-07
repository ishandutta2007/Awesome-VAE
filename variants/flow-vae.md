# Normalizing Flow VAE

Normalizing Flow VAEs combine the VAE framework with Normalizing Flows to transform a simple latent distribution (like a Gaussian) into a highly complex and expressive one.

## 🏗️ Architecture Diagram
*(Diagram to be added)*

## 🔑 Key Features
- **Invertible Transformations:** Passes the latent variable through a sequence of invertible mathematical functions.
- **Complex Latent Shapes:** Can model multi-modal or highly skewed distributions that a standard Gaussian cannot capture.
- **Differentiable Mapping:** The Jacobian determinant of the flow allows for exact density estimation.

## 📝 Research Paper
*   [Variational Inference with Normalizing Flows (Rezende & Mohamed, 2015)](https://arxiv.org/abs/1505.05770)

---
[⬅️ Back to README](../README.md)
