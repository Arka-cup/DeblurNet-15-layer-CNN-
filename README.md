# DeblurNet-15-layer-CNN-
# DeblurNet: 15-Layer CNN for Image Deblurring (Inspired by SRCNN)

This project implements a **15-layer deep convolutional neural network** for **image deblurring**, built in **PyTorch**.  
The architecture is **inspired by SRCNN (Super-Resolution Convolutional Neural Network)** but extended with more layers, bottleneck blocks, and deeper feature extraction to handle motion blur and restore sharpness.

---

## ✨ Features
- **15-layer DeblurCNN**, extended from classic SRCNN
- **Smart dataset pairing** (matches blur/sharp images by filename normalization, falls back to index-based pairing)
- **Customizable training**: epochs, batch size, learning rate, image size
- **Periodic checkpoints** with saved preview images (blur → deblur → sharp)
- **Loss plots** (`loss.png`) for monitoring training
- **GPU acceleration** (CUDA support)
- **Reproducibility** with fixed random seed

---

## 📂 Project Structure
deblur-net/
├─ deblur_train_full.py # Main training script
├─ requirements.txt # Python dependencies
├─ README.md # Documentation
├─ .gitignore # Ignore data/outputs/checkpoints
├─ data/
│ ├─ blur/ # Input blurred images
│ └─ deblur/ # Ground-truth sharp images
└─ outputs/
├─ saved_images/ # Preview results during validation
├─ loss.png # Training vs validation loss curve
└─ model.pth # Final trained model


---

## 🚀 Setup

### 1. Clone the repo
```bash
git clone https://github.com/<your-username>/deblur-net.git
cd deblur-net

🛠️ Requirements

Python 3.8+

PyTorch ≥ 1.12

torchvision

OpenCV

scikit-learn

matplotlib

tqdm

Acknowledgements

SRCNN: Dong et al., “Image Super-Resolution Using Deep Convolutional Networks” (2014)(https://debuggercafe.com/srcnn-implementation-in-pytorch-for-image-super-resolution/)

PyTorch, torchvision, OpenCV, scikit-learn

Dataset Link = "https://www.kaggle.com/datasets/kwentar/blur-dataset?utm_source=chatgpt.com"

