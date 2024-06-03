# Binary Classification of CIFAR-10 Dataset

## Objective
This project involves classifying images from the CIFAR-10 dataset into two categories:
- **Can Fly**: Bird and Airplane
- **Cannot Fly**: Frog, Deer, Truck

## Dataset
The CIFAR-10 dataset consists of 60,000 32x32 color images in 10 different classes, with 6,000 images per class. For this project, we filter the dataset to focus on the relevant classes for our binary classification task.
![alt text](https://raw.githubusercontent.com/rnoxy/cifar10-cnn/master/img/cifar10-examples.png)


## Model Architecture
We used a Convolutional Neural Network (CNN) for the classification task. The architecture includes:
- Input layer with shape (32, 32, 3)
- Three convolutional layers with ReLU activation and max pooling
- Dropout layers for regularization
- Fully connected (dense) layer with ReLU activation
- Output layer with sigmoid activation for binary classification

## Training
The model is trained using the following configuration:
- **Loss Function**: Binary Crossentropy
- **Optimizer**: Adam
- **Metrics**: Accuracy
- **Batch Size**: 32
- **Epochs**: 10
- **Validation Split**: 20%

## Evaluation
The model is evaluated using the confusion matrix, which helps in understanding the model's performance in terms of true positives, true negatives, false positives, and false negatives.

## Performance Metrics
- **Accuracy**: 88.74%
- **Precision**: 77.78%
- **Recall**: 61.2%
- **F1 Score**: 68.4%
