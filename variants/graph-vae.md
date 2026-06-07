# Graph VAE (GVAE / VGAE)

Graph Variational Autoencoders are designed to process non-Euclidean data structured as graphs, learning to encode and reconstruct nodes and edges.

## 🏗️ Architecture Diagram
![VGAE Architecture](https://miro.medium.com/v2/resize:fit:1400/1*8_8_8_8_8_8_8_8_8_8_8.png)

## 🔑 Key Features
- **Graph Convolutional Networks (GCN):** Uses GCNs as the encoder to capture local neighborhood information.
- **Adjacency Matrix Reconstruction:** The decoder typically aims to reconstruct the original graph's adjacency matrix.
- **Relational Learning:** Excellent for molecular generation, citation networks, and social link prediction.

## 📝 Research Paper
*   [Variational Graph Auto-Encoders (Kipf & Welling, 2016)](https://arxiv.org/abs/1611.07308)

---
[⬅️ Back to README](../README.md)
