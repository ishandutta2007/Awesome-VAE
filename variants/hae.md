# Hierarchical VAE (HVAE / H-VAE)

Hierarchical VAEs use multiple layers of latent variables to capture data features at different levels of abstraction, from global structure to fine-grained details.

## 🏗️ Architecture Diagram
*(Diagram to be added)*

## 🔑 Key Features
- **Layered Representation:** Stacks multiple latent layers, where each layer is conditioned on the previous one.
- **Deep Latent Space:** Can model much more complex distributions than a standard "shallow" VAE.
- **Ladder Structure:** Often implemented using "Ladder" connections to share information between bottom-up and top-down paths.

## 📝 Research Paper
*   [Ladder Variational Autoencoders (Sønderby et al., 2016)](https://arxiv.org/abs/1602.02282)

---
[⬅️ Back to README](../README.md)
