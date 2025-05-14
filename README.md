# Deep Learning Mini Project 3 – Adversarial Attacks on ImageNet Models

This repository contains the final mini-project submission for CS-GY 6953 / ECE-GY 7123 (Spring 2025), focused on evaluating and implementing adversarial attacks on pretrained deep neural networks.

## 📌 Project Overview

We investigate the vulnerability of production-grade image classifiers to various adversarial attacks using a subset of ImageNet-1K.

### 🔍 Tasks Covered

- **FGSM Attack**  
  Fast Gradient Sign Method to perturb inputs within an L∞ norm constraint.

- **Iterative/PGD Attacks**  
  Stronger iterative variants that improve degradation while maintaining same ε.

- **Patch-Based Attacks**  
  Localized occlusions to mislead models, evaluating limitations of spatial masking.

- **Transferability Analysis**  
  Testing how adversarial samples transfer from ResNet-34 to other models like DenseNet-121.

---

## 🧠 Models Used

- ResNet-34 (ImageNet pretrained)
- DenseNet-121 (for transferability study)

---
## 📈 Result
Transferability Results:
| Dataset               |   Top-1 (%) |   Top-5 (%) |
|:----------------------|------------:|------------:|
| Clean                 |         0   |         0   |
| Adv Set 1 (FGSM)      |        45.8 |        76.2 |
| Adv Set 2 (PGD)       |        47.8 |        81.4 |
| Adv Set 3 (Patch-PGD) |        74.8 |        93.2 |

![Screenshot 2025-05-14 161250](https://github.com/user-attachments/assets/a19f16f8-cf45-46a3-9c70-c60b774f189a)

