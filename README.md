# MedMNIST-LSGAN-WGAN-GP# 
This repository compares three Generative Adversarial Network (GAN) architectures — **LSGAN**, **WGAN**, and **WGAN-GP** — on the [PneumoniaMNIST](https://medmnist.com/) dataset. The aim is to generate realistic synthetic chest X-ray images and evaluate them using standard GAN evaluation metrics and TensorBoard visualization.

---

## 📊 Dataset: PneumoniaMNIST

- **Source**: MedMNIST - https://medmnist.com/
- **Type**: 28x28 grayscale chest X-rays
- **Classes**: Binary — Pneumonia (1) vs Normal (0)
- **Split**:
  - Train: 5,856 images
  - Validation: 1,496 images
  - Test: 1,498 images

---

## 🧠 Implemented GAN Models

| Model     | Description |
|-----------|-------------|
| **LSGAN** | Uses Least Squares loss for smoother training and better gradients |
| **WGAN**  | Replaces binary loss with Wasserstein distance for improved convergence |
| **WGAN-GP** | Improves WGAN by adding a gradient penalty to enforce Lipschitz constraint |

✅ All models share the same generator and discriminator architecture for fairness.

---

## 🚀 Installation

```bash
git clone https://github.com/Sarveshap/LSGAN-vs-WGAN-vs-WGAN-GP-MedMNIST.git
cd LSGAN-vs-WGAN-vs-WGAN-GP-MedMNIST
pip install -r requirements.txt
