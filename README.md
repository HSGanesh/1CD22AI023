# CIFAR-10 Image Classification using CNN (TensorFlow / Keras)

This project implements a **Convolutional Neural Network (CNN)** for **multi-class image classification** using the **CIFAR-10 dataset**.  
The implementation is **modified and extended** from an original **Cats vs Dogs (binary classification)** CNN codebase.

The key improvement is adapting the model for **10-class classification** and adding **model persistence** to avoid retraining in Google Colab.

---

##  Original Code Reference
The original code was designed for:
- **Binary classification (Cats vs Dogs)**
- Directory-based image loading
- Sigmoid output with binary cross-entropy loss

---

##  Modifications Made (IMPORTANT)

### 1️ Dataset Changed
**Original:**
- Cats vs Dogs dataset
- Images loaded from directories using `ImageDataGenerator`

**Modified:**
- **CIFAR-10 dataset**
- Loaded directly using:
```python
from tensorflow.keras.datasets import cifar10
