# Conditional VAE (CVAE)

CVAE is a type of VAE that allows for controlled data generation by conditioning the encoding and decoding processes on external information, such as class labels or text descriptions.

## 🏗️ Architecture Diagram
![CVAE Architecture](https://www.researchgate.net/profile/Sushan-Nakarmi/publication/331234567/figure/fig1/AS:11431281234567168@1712640000000/Schematic-of-the-conditional-variational-autoencoder-cVAE.png)

## 🔑 Key Features
- **Targeted Generation:** By providing a label (e.g., "generate a digit 7"), the model can produce specific classes of output.
- **Label Conditioning:** Labels are typically concatenated with the input data for the encoder and with the latent vector for the decoder.
- **Versatility:** Used extensively in text-to-image synthesis and controlled speech generation.

## 📝 Research Paper
*   [Learning Structured Output Representation using Deep Conditional Generative Models (Sohn et al., 2015)](https://proceedings.neurips.cc/paper/2015/hash/8d55a249e6baa5c06772297520da2051-Abstract.html)

---
[⬅️ Back to README](../README.md)
