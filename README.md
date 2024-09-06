# Enhancing Handwritten Character Recognition: A Comparative Study of Normalization and Pooling Techniques
## Overview
This repository contains a research study and implementation for handwritten character recognition. The study explores and compares the effectiveness of different normalization techniques—Global Max Pooling, Batch Normalization, and Layer Normalization—in improving the accuracy of handwritten character recognition using a Convolutional Neural Network (CNN). The dataset used is the A_Z Handwritten Data.csv, which includes handwritten images of each letter from A to Z.
## Abstract
Handwritten character recognition (HCR) presents significant challenges due to the variability in individual handwriting styles. This project evaluates and compares the effectiveness of three different techniques—Batch Normalization, Layer Normalization, and Global Max Pooling—using the A_Z Handwritten Data.csv dataset, which includes diverse examples of handwritten alphabets. The analysis demonstrates that Layer Normalization achieves the highest accuracy, reaching 99.98%. This result highlights the superior performance of Layer Normalization in improving the reliability and efficiency of handwritten character recognition systems.
## Dataset
- Name: A_Z Handwritten Data.csv
- Source: Kaggle
- Description: The dataset consists of grayscale handwritten images representing alphabets A to Z. Each letter is contained in a 20x20 pixel square, centered, and saved in PNG format with 28x28 size.
- Format: CSV to image conversion performed with preprocessing steps.
## Model Architecture
The model is a Convolutional Neural Network (CNN) designed for handwritten character recognition, incorporating various types of layers to extract features and perform classification. The architecture was evaluated using different techniques, including Global Max Pooling, Batch Normalization, and Layer Normalization. Layer Normalization was found to offer the highest accuracy, leading to its detailed presentation here. Below is a summary of the architecture:

### Convolutional Layers
- Convolutional Layers: Multiple Conv2D layers with increasing filter sizes (32, 64, 128) are used to extract features from the images. These layers help in detecting various patterns and details in the images.

- Layer Normalization: Applied after each convolutional layer to stabilize and accelerate training by normalizing the activations.

- Max Pooling Layers: MaxPooling2D layers are used to reduce the spatial dimensions of the feature maps, helping to retain the most important features while reducing computational complexity.

### Dense Layers
- Flattening Layer: Converts the 3D feature maps into a 1D vector to prepare for the fully connected layers.

- Dense Layers: Several Dense layers (with 256 and 128 neurons) are used for high-level reasoning and classification. Dropout is applied in these layers to prevent overfitting.

- Output Layer: The final Dense layer with 26 neurons corresponds to the 26 classes (letters A-Z) in the dataset.
### Model Summary

![Model Summary](https://github.com/user-attachments/assets/ed4ac383-b1e5-45f5-af7a-d1a59a9a043d)


## Model Performace 
The model is trained for 50 epochs, allowing sufficient iterations for the network to learn and generalize from the data. This extended training period helps achieve better convergence and fine-tune the model's parameters for optimal performance.

![epoch 50](https://github.com/user-attachments/assets/56956c07-fc8a-46ca-922c-edec4c1d1774)


## Conclusion
This project undertook a comparative analysis of three normalization techniques—Global Max Pooling, Batch Normalization, and Layer Normalization—for handwritten character recognition. The findings reveal that Layer Normalization significantly outperforms the other methods, achieving a remarkable accuracy of 99.98% on the A_Z Handwritten Data.csv dataset. This highlights Layer Normalization's superior effectiveness in refining the accuracy of character recognition systems.

The study underscores the importance of choosing the right normalization approach to enhance performance. Future research should aim to further investigate and optimize these techniques, exploring their potential for broader applications and improving the robustness of handwritten text recognition systems. This work demonstrates the critical role of advanced normalization strategies in advancing the field of character recognition.

## Impact
The success of Layer Normalization in this study demonstrates its potential for creating more accurate and reliable character recognition systems. This advancement is valuable for applications that rely on precise interpretation of handwritten text, offering substantial improvements in efficiency and accuracy.

## Acknowledgments
- Kaggle for providing the dataset.
- The developers and researchers contributing to CNN and normalization techniques.

