# Cat-and-Dog-Image-Classification-Using-CNN-Convolutional-Neural-Network

# Dogs vs. Cats Image Classification

## Project Overview

This project demonstrates a deep learning pipeline to classify images of dogs and cats using Convolutional Neural Networks (CNNs). The model is trained on the Kaggle "Dogs vs. Cats" dataset, with performance evaluated before and after applying regularization techniques such as Batch Normalization and Dropout. Visualization of overfitting is included through training and validation accuracy/loss plots, along with predictions on custom cat and dog images.

---

## Features

### 1. Dataset
- Utilizes the "Dogs vs. Cats" dataset from Kaggle.
- Images are organized into `train` and `test` directories for training and validation.

### 2. Model Architecture
#### Initial Model:
- Three convolutional layers with ReLU activation.
- MaxPooling layers after each convolutional block.
- Fully connected dense layers with a sigmoid output for binary classification.

#### Enhanced Model:
- Batch Normalization applied after each convolutional block.
- Dropout layers added to reduce overfitting.

### 3. Training Pipeline
- Images are preprocessed by normalizing pixel values to [0, 1].
- Model is trained with `binary_crossentropy` as the loss function and `adam` optimizer.
- Training and validation accuracy/loss are visualized to analyze overfitting and improvements.

### 4. Overfitting Analysis
- **Before Applying Regularization:**
  - Plots show a significant gap between training and validation accuracy/loss, indicating overfitting.

  - Accuracy (red) and Val_Accuracy (blue)
   ![image](https://github.com/user-attachments/assets/5c3b128b-b47c-46b5-b8ce-29bd3233273f)
  <br>
  - Loss (red) and Val_Loss (blue)
  ![image](https://github.com/user-attachments/assets/874b748a-4ceb-49da-9f17-0988b2af7caa)

    
- **After Applying Batch Normalization and Dropout:**
  - Plots demonstrate improved generalization, with reduced overfitting and better alignment of training and validation curves.

### 5. Custom Image Prediction
- Includes functionality to test the trained model on custom cat and dog images.
- Predicts whether an image is of a dog or a cat and displays the result.

---

## Visualizations

### Overfitting Analysis
1. **Before Applying Regularization:**
   - Training and validation accuracy and loss curves highlight overfitting.
  
  
     
2. **After Applying Regularization:**
   - Improved curves with reduced overfitting.
