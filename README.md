# 🧠 AttentiveHybridNet

<div align="center">

**Hybrid Deep Learning for Brain Tumor Classification**

[![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0+-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)](https://pytorch.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](LICENSE)

**Accuracy: 96.37% | ECE < 0.03 

</div>

---

## 🌟 Overview

AttentiveHybridNet combines **ResNet-18** and **Swin Transformer** using a novel cross-attention mechanism to classify brain tumors from MRI scans with **96.37% accuracy**.

### ✨ Key Features

🔹 **Dual-Branch Architecture** - CNN + Transformer for comprehensive feature extraction  
🔹 **Cross-Attention Fusion** - Smart feature integration  
🔹 **Grad-CAM Visualization** - Interpretable AI for clinical trust  
🔹 **Robust Validation** - 5-fold cross-validation  

---

## 📊 Performance

### 🏆 Our Results

| Model | Accuracy | F1-Score | Improvement |
|-------|----------|----------|-------------|
| ResNet-18 | 87.11% | 87.05% | baseline |
| Swin Transformer | 94.88% | 94.85% | +7.77% |
| Concatenation Fusion | 94.25% | 93.92% | +7.14% |
| **AttentiveHybridNet** ⭐ | **96.37%** | **96.38%** | **+9.26%** |

### 📈 State-of-the-Art Comparison

| Study | Accuracy |
|-------|----------|
| Lu et al. (2025) | 96.3% |
| **AttentiveHybridNet (Ours)** | **96.37%** ⭐ |
| Tariq et al. (2025) | 96.0% |
| Yoon (2025) | 94.85% |

---

## 🚀 Quick Start

### Installation

```bash
git clone https://github.com/HimaniMahajan27/AttentiveHybridNet.git
cd AttentiveHybridNet
pip install -r requirements.txt
```

### Train the Model

```python
python train.py --data_dir ./data --epochs 100 --batch_size 16
```

### Test & Visualize

```python
python test.py --model_path ./checkpoints/best_model.pth
python inference.py --image_path test.jpg --grad_cam
```

---

## 🏗️ Architecture

```
Input MRI (224×224)
    ├── 🔵 ResNet-18 → Local Features (512-dim)
    ├── 🟢 Swin Transformer → Global Context (768-dim)
    └── 🔶 Cross-Attention Fusion → 3 Classes
```

**Classes**: Glioma | Meningioma | Pituitary




---

## 👩‍💻 Author

<div align="center">

**Himani Mahajan**

Computer Engineering | Thapar Institute of Engineering & Technology

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/himani-mahajan-9553732ab/)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/HimaniMahajan27)

</div>

---



<div align="center">

⭐ **Star this repo if you find it helpful!** ⭐

**Made with ❤️ by Himani Mahajan**

</div>
