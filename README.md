# CIFAR-10 Classification Using CNN

## Objective
The objective of this project is to effectively classify images into 10 different classes: ["aeroplane", "automobile", "bird", "cat", "deer", "dog", "frog", "horse", "ship", "truck"] using Convolutional Neural Networks (CNNs).

## Dataset
- The CIFAR-10 dataset consists of 50,000 training images and 10,000 test images.
- All images are resized to 32 x 32 pixels.
- The dataset is shuffled to prevent overfitting and encourage generalization.

## Model Selection
- CNNs are chosen over ANNs due to the dataset size and the aim for maximum accuracy.
- Various models are trained with different configurations of dense layers, layer sizes, and convolutional layers.
- Hyperparameter tuning is performed to optimize the model.

## Best Model
Using tuner search and random searching, the parameters of the best model are determined to be:
- Number of convolutional layers: 3
- Number of convolutional filters: 96
- Number of dense layers: 2
- Number of dense units: 3000

![Best Model Parameters](https://github.com/AniruthSuresh/CIFAR---10-Classification/assets/137063103/9e8ffddc-688b-4a48-9bdf-7de28d1d0cec)

## Convolutional Network
1. Sequential model components:
   - Convolutional layer with a kernel size of (3,3) and 64 filters.
   - Max pooling layer to improve feature mapping and reduce data size.
2. Output layer:
   - Utilizes a linear activation function with 10 units for classification.
   - Softmax activation function is used to predict the probabilities of each class.

## Performance
The model achieves the following metrics on the test data:
- Accuracy: 67.77%
- Loss: 0.998

This implementation demonstrates effective image classification using CNNs on the CIFAR-10 dataset.

