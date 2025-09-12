# Experiment 3: Perceptron vs Multilayer Perceptron (A/B Test)

## Objective

Compare the performance of two models:

- **PLA (Perceptron Learning Algorithm)**: A single-layer model with step activation.
- **MLP (Multilayer Perceptron)**: A neural network with hidden layers and non-linear activation functions.

---

## Dataset

- **Name**: English Handwritten Characters Dataset  
- **Size**: 3,410 images  
- **Classes**: 62 (0–9, A–Z, a–z)

---

## Preprocessing

- Resize images (e.g., 28x28)
- Flatten to 1D vectors
- Normalize pixel values to [0, 1]
- Split into train, validation, and test sets

---

## PLA (Perceptron Learning Algorithm)

- **Activation**: Step function  
- **Update Rule**:  
  `w(t+1) = w(t) + η * (y - ŷ) * x`
- **Limitation**: Only works well for linearly separable data

---

## MLP (Multilayer Perceptron)

- **Layers**: Input → Hidden → Output
- **Activations**: ReLU, Tanh, Sigmoid (tested)
- **Loss Function**: Cross-Entropy
- **Optimizers**: SGD, Adam

### Tuned Hyperparameters

- **Hidden layers**: 2  
- **Neurons per layer**: 128, 64  
- **Activation**: ReLU  
- **Optimizer**: Adam  
- **Learning Rate**: 0.001  
- **Batch Size**: 64  

---

## Results Summary

| Metric       | PLA  | MLP  |
|--------------|------|------|
| Accuracy     | Low  | High |
| Convergence  | Slow | Fast |
| Flexibility  | Low  | High |

---

## Key Observations

- PLA performs poorly due to data not being linearly separable.
- MLP outperforms PLA by learning complex patterns.
- Optimizer and activation choice significantly affect MLP performance.
- Too many layers can cause overfitting.
