# 🧠 MNIST CNN Classifier & Deployment Pipeline (PyTorch → ONNX)

This project documents my journey building a high-accuracy convolutional neural network (CNN) using PyTorch, then optimizing it through **quantization** and **ONNX export** — skills directly aligned with the USAF/MIT **Phantom AI – Fast AI track**.

---

## ✅ What I Built

- A clean CNN trained on the MNIST dataset, achieving **99.3% test accuracy**
- Model optimization using **PyTorch dynamic quantization** (↓71% model size)
- Deployment-ready model via **ONNX export + post-export quantization**
- Inference validation using **ONNX Runtime**

---

## 🧠 Skills & Concepts Practiced

- CNN design for image classification
- Training pipelines with PyTorch (data loaders, GPU acceleration)
- Performance tuning (Adam optimizer, dropout, normalization)
- Model compression with `torch.quantization`
- ONNX model export and quantization via `onnxruntime`
- Inference execution outside PyTorch

---

## 📁 File Overview

| File | Description |
|------|-------------|
| `MNIST_CNN_Training.ipynb` | CNN architecture, training loop, and evaluation (Day 1) |
| `Model_Quantization_ONNX.ipynb` | PyTorch → ONNX quantization + runtime validation (Day 2) |
| `requirements.txt` | All necessary libraries |

---

## 🔢 Results

| Model            | Accuracy | Size   | Size ↓ |
|------------------|----------|--------|--------|
| Full PyTorch     | 99.3%    | 1650KB | —      |
| Quantized (Torch)| 99.3%    | 472KB  | ↓71%   |
| Quantized (ONNX) | 99.3%    | 472KB  | ↓71%   |

---

## 📦 Why This Matters for Fast AI

This work mimics real-world constraints in DoD/edge AI deployments:

- **Training → Portability → Inference**
- Compressing models without accuracy loss
- Deploying to environments where **Python is not available**
- Demonstrating **ONNX mastery** — a key Fast AI track objective

---

## 🚀 Next Steps

- Benchmark CPU vs quantized ONNX inference latency
- Explore TensorRT and OpenVINO backends
- Package for deployment (e.g., REST API or embedded device)
- Extend to multi-digit MNIST or CIFAR10

---

🛠️ *Built and maintained by Armand Debray*  

