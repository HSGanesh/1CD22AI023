##  Modifications Made (IMPORTANT)

The following **intentional and justified changes** were made to the original AlexNet:

### 1️ Reduced Kernel Size in First Convolution Layer
**Original:** `11 × 11` kernel  
**Modified:** `7 × 7` kernel  

 Reduces computational cost  
 Preserves spatial information  

---

### 2️ Added Batch Normalization
Batch Normalization layers were added after major convolution layers.

- Improves training stability  
- Speeds up convergence  
- Reduces internal covariate shift  

---

### 3️ Reduced Fully Connected Layer Size
**Original:**  
- Dense(4096) → Dense(4096)

**Modified:**  
- Dense(1024) → Dense(1024)

- Reduces number of parameters  
- Prevents overfitting  
- Suitable for smaller datasets  

---

### 4️ Increased Dropout Regularization
Dropout rate increased to **0.6**.

- Improves generalization  
- Reduces overfitting  

---

### 5️ Configurable Output Classes
The output layer is now configurable using `num_classes`.

- Can be used for CIFAR-10 or custom datasets  
- Not restricted to ImageNet  

---

## Final Model Architecture
- Convolutional layers with ReLU activation
- MaxPooling layers for spatial reduction
- Batch Normalization for stability
- Fully connected dense layers
- Softmax output layer for multi-class classification
