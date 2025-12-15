# Character-Level Text Generation using RNN

This project implements a **character-level text generation model** using a **Recurrent Neural Network (RNN)** in TensorFlow/Keras.  
The model learns character patterns from a given input sentence and generates new text character by character.

---

##  Objective
To understand how **Recurrent Neural Networks (RNNs)** can be used for sequential data modeling and text generation at the character level.

---

##  Original Code Overview
The original implementation:
- Used a SimpleRNN layer
- Performed one-hot encoding of characters
- Generated text using greedy (argmax) sampling
- Had minimal regularization

---

##  Modifications Made (IMPORTANT)

The following **meaningful improvements** were introduced:

### 1️ Modular Data Preparation
- Dataset creation was moved into a separate function
- Improves readability and reusability

### 2️ Improved RNN Activation Function
- Changed activation from `relu` to `tanh`
- `tanh` is better suited for recurrent architectures

### 3️ Added Dropout Regularization
- Dropout layer added after the RNN
- Reduces overfitting on small text data

### 4️ Temperature-Based Sampling
- Replaced greedy sampling with temperature-controlled sampling
- Allows control over randomness and creativity in generated text

### 5️ Hyperparameter Organization
- Sequence length, epochs, and temperature grouped as configurable parameters

---

##  Model Architecture
- SimpleRNN layer (50 units, tanh activation)
- Dropout layer (0.2)
- Dense output layer with softmax activation

---

##  Training Details
- Sequence length: 5 characters
- Epochs: 100
- Loss function: Categorical Crossentropy
- Optimizer: Adam

---

##  Output
- Generated text based on a given starting sequence
- Character-by-character prediction using trained RNN

---

##  Technologies Used
- Python
- NumPy
- TensorFlow / Keras
- Recurrent Neural Networks (RNN)
