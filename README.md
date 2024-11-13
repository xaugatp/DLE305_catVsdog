

# **Cat vs Dog Image Classification**

This project focuses on developing and evaluating various deep learning models for classifying images of cats and dogs. The goal is to explore how increasing the depth and complexity of Convolutional Neural Networks (CNNs) affects their classification performance, efficiency, and computational requirements.

---

## **Table of Contents**
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Model Architectures](#model-architectures)
4. [Results](#results)
5. [Dependencies](#dependencies)
6. [Author](#author)


---

## **Project Overview**

This project explores the use of deep learning techniques for binary image classification of cats and dogs. Starting with a simple Multi-Layer Perceptron (MLP) as a baseline, we experimented with various CNN architectures, including a VGG-like model and a more complex 5-layer "Huge" model. The models were implemented using TensorFlow and trained to optimize accuracy while considering computational efficiency.

## **Dataset**

The dataset used in this project consists of labeled images of cats and dogs, containing:
- **10,015** dog images
- **9,985** cat images

### **Data Preprocessing**
- Images were resized to a standard dimension of **150x150 pixels**.
- Normalization was applied to scale pixel values to the range [0, 1].
- The data was split into training and validation sets.

## **Model Architectures**

We experimented with the following models:
1. **Multi-Layer Perceptron (MLP)**
   - Achieved ~50% validation accuracy.
   - Baseline model for comparison.

2. **Single-Layer CNN**
   - Consisted of one convolutional layer.
   - Achieved **68%** validation accuracy.

3. **Two-Layer CNN**
   - Achieved **~70%** validation accuracy.
   - Balanced feature extraction with computational efficiency.

4. **VGG-Like CNN**
   - Inspired by the VGG architecture.
   - Achieved **94%** validation accuracy.
   - Required higher computational resources.

5. **"Huge" Model (5-Layer CNN)**
   - Achieved the highest accuracy of **95%**.
   - Most resource-intensive model with diminishing returns on accuracy improvements.

## **Results**

| **Model**            | **Validation Accuracy** | **Strengths**                 | **Limitations**                      |
|----------------------|-------------------------|------------------------------|-------------------------------------|
| MLP                  | ~50%                    | Lightweight, easy to implement | Poor spatial feature extraction     |
| Single-Layer CNN     | 68%                     | Good initial improvement     | Limited depth                       |
| Two-Layer CNN        | ~70%                    | Balanced performance & efficiency | Limited generalization             |
| VGG-Like Model       | 94%                     | High accuracy, robust feature extraction | High computational demands  |
| "Huge" Model         | 95%                     | Highest accuracy achieved    | Very resource-intensive             |

## **Dependencies**

To run this project, you will need the following libraries:
- Python 3.8+
- TensorFlow 2.10+
- NumPy
- Pandas
- Matplotlib
- scikit-learn







## **Author**
- Saugat Poudel
- Email: saugat.poudel@student.torrens.edu.au


Feel free to update the sections with specific paths, model names, and links relevant to your project.
