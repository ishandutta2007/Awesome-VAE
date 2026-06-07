# VQ-VAE-2

VQ-VAE-2 is a hierarchical extension of the original VQ-VAE, designed to generate high-resolution images by capturing both global structures and local details across multiple scales.

## 🏗️ Architecture Diagram
*(Diagram available in the research paper below)*
> [View Diagram in Paper (Figure 2)](https://arxiv.org/pdf/1906.00446.pdf#page=3)

## 🔑 Key Features
- **Multi-Scale Codebooks:** Uses a hierarchical latent space with top-level codebooks for global features and bottom-level codebooks for fine-grained details.
- **High-Resolution Synthesis:** Capable of generating diverse, high-fidelity images at 256x256 or higher.
- **Powerful Prior:** Typically uses a PixelCNN or Transformer as a prior over the discrete codes.

## 📝 Research Paper
*   [Generating Diverse High-Fidelity Images with VQ-VAE-2 (Razavi et al., 2019)](https://arxiv.org/abs/1906.00446)

---
[⬅️ Back to README](../README.md)
