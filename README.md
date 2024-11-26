# Fashion MNIST Dataset Analysis and Modeling

This notebook demonstrates an end-to-end implementation for analyzing and classifying the **Fashion MNIST Dataset** using a Convolutional Neural Network (CNN).

---

## Key Sections

### 1. Introduction
- **Problem Statement**: Classify images from the Fashion MNIST dataset, which contains 70,000 grayscale images (28x28 pixels) across 10 fashion categories.

---

### 2. Environment Setup
- Imported libraries: `TensorFlow`, `NumPy`, `Pandas`, `Matplotlib`, and `Seaborn`.

---

### 3. Dataset Loading
- Loaded using TensorFlow's `fashion_mnist` module.
- Split into:
  - **Training set**: 60,000 samples.
  - **Testing set**: 10,000 samples.

---

### 4. Data Exploration
- **Category descriptions**:
  - 0: T-shirt/top
  - 1: Trouser
  - 2: Pullover
  - 3: Dress
  - 4: Coat
  - 5: Sandal
  - 6: Shirt
  - 7: Sneaker
  - 8: Bag
  - 9: Ankle Boot
- Random image samples and labels are visualized.

---

### 5. Model Building
- A **Convolutional Neural Network (CNN)** was built using TensorFlow's Keras API.
- **Key Features**:
  - **Normalization**: Input data scaled to [0, 1].
  - Layers:
    - Convolutional layers with filters and ReLU activation.
    - Max pooling for down-sampling.
    - Fully connected dense layers.
  - Compiled with:
    - Optimizer: `Adam`
    - Loss function: `sparse_categorical_crossentropy`
    - Metrics: Accuracy.

---

### 6. Training
- Trained over 150 epochs with **early stopping** to prevent overfitting.
- Tracked:
  - **Training loss**
  - **Validation loss**

---

### 7. Evaluation
- Achieved **91% accuracy** on the test set.
- Generated:
  - Confusion matrix heatmap for category-wise performance.
  - Classification report with precision, recall, and F1-score.

---

### 8. Visualizations
- Plotted **training and validation loss** across epochs.
- Visualized the **confusion matrix** as a heatmap.

---

### 9. Insights and Observations
- **Model Performance**:
  - High accuracy (91%) with minimal overfitting.
  - Training loss decreased steadily, indicating effective learning.
  - Validation loss stabilized early, suggesting generalization.
- **Classification Metrics**:
  - Precision, recall, and F1-score consistent across categories.

---

### 10. Final Inference
- The CNN model effectively classifies the Fashion MNIST dataset, demonstrating strong performance and reliability.

---
