# Vision From Scratch

> **Learning Computer Vision from the ground up by implementing foundational and State-of-the-Art (SOTA) research papers entirely from scratch in PyTorch.**

This repository is a personal deep dive into the mechanics of Computer Vision architectures. Instead of relying on high-level APIs or pre-built models, the goal is to translate complex mathematical methodologies and architectural diagrams from research papers directly into raw, understandable code.

---

## 🚀 Implemented Architectures

### 1. Vision Transformer (ViT)
* **Paper:** [An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale](https://arxiv.org/abs/2010.11929)
* **Status:** ✅ Implemented
* **Highlights:**
  * Custom Patch Embedding using `Conv2d` stride tricks.
  * Multi-Head Self Attention (MHA) with single-layer QKV optimization.
  * Standardized Transformer Encoder blocks with Pre-Norm architecture.
  * Evaluated on CIFAR-10.

### 2. Data-efficient Image Transformers (DeiT)
* **Paper:** [Training data-efficient image transformers & distillation through attention](https://arxiv.org/abs/2012.12877)
* **Status:** ✅ Implemented
* **Highlights:**
  * Dual-token architecture (`cls_token` and `dist_token`).
  * Custom **Hard Distillation Loss** function matching the paper's mathematical formulation.
  * Advanced Optimizer grouping (separating weight decay for specific parameters).
  * Evaluated on CIFAR-10 using both CNN (ResNet) and Transformer (ViT) teacher models.

---

## 📂 Repository Structure

```text
Vision-From-Scratch/
├── notebooks/           # Interactive Jupyter/Colab notebooks for training and evaluation
    ├── ViT_CIFAR10.ipynb
    └── DeiT_CIFAR10.ipynb

```
### Tech Stack & Requirements
Framework: PyTorch

Libraries: torchvision, timm, matplotlib

### Environment: Designed and tested in Google Colab (T4 GPU)

### What's Next?
Future implementations planned for this repository:

[ ] Swin Transformer

[ ] ConvNeXt

[ ] Masked Autoencoders (MAE)

Created for the purpose of learning, debugging, and demystifying AI.
