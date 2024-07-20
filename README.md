# Pneumonia Detection Using Convolutional Neural Networks (CNNs)

## Overview
This project aims to develop a robust Convolutional Neural Network (CNN) model to classify chest X-ray images as indicative of pneumonia or normal. The model is trained on a well-curated dataset of chest X-ray images and evaluated based on key performance metrics to ensure accuracy and reliability.

## Dataset
**Dataset**: ChestX-ray14  
**Image Preprocessing**: Images were preprocessed using resizing (120x120 pixels), normalization (rescaling to 1/255), and no augmentation.

## Methodology

### Image Preprocessing
- **Resizing**: Standardized image size to 120x120 pixels for uniformity.
- **Normalization**: Pixel values normalized to the range 0-1 to facilitate faster and more stable convergence.

### Model Architecture
- **CNN Architecture**: A custom CNN architecture was used with 5 convolutional layers, each followed by max pooling. The final layers include a flatten layer, two dense layers with ReLU activation, and an output layer with sigmoid activation for binary classification.

### Training
- **Data Split**: The dataset was divided into training (80%), validation (10%), and testing (10%) sets.
- **Hyperparameters**: 
  - Optimizer: Adam
  - Learning rate: 0.001
  - Loss function: Binary cross-entropy
- **Training Process**: The model was trained for 10 epochs with a batch size of 8.

### Evaluation
- **Metrics**: The model's performance was evaluated using accuracy, loss, precision, recall, and F1-score on the test set.
- **Results**: 
  - Accuracy: 78.6%
  - Loss: 1.3276

## Conclusion
The developed CNN model demonstrates promising performance in classifying chest X-ray images as pneumonia or normal. The model's accuracy and other evaluation metrics indicate its potential for assisting in medical diagnosis. However, further research and development are necessary to enhance the model's robustness and reliability in real-world clinical settings.
