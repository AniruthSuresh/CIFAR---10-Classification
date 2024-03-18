
# CIFAR---10-Classification-Using-CNN

- **Objective**:
  - The objective here is to effectively classify 10 outcomes : ["aeroplane","automobile","bird","cat","deer","dog","frog","horse","ship","truck"]
    
- **Dataset**:
  - We utilized the standard CIFAR - 10 dataset that has 50000 train images and 10000 test images 
  - All images were scaled to the size of 32 x 32 pixels.
  - The dataset was shuffled to prevent the model from memorizing and encourage understanding.

- **Model Selection**:
  - Due to the dataset's size and the aim for maximum accuracy, **Convolutional Neural Networks (CNNs)** were chosen over Artificial Neural Networks (ANNs).
  - Various models were trained, considering different configurations of dense layers, layer sizes, and convolutional layers.
  - Dense layer options: [0, 1, 2]
  - Layer sizes options: [32, 64, 128]
  - Convolutional layer options: [1, 2, 3]
  - 27 models were tested, and their performance was evaluated using **Tensorboard**.

- **Best Model**:
  - The model with **2 dense layers with 3000 and 1000 units respectively , a conv layer size of 64, and 3 convolutional layers** emerged as the best fit for our dataset.

- **Convolutional Network**:
  1. We constructed a sequential model with the following components:
     - Convolutional layer with a kernel size of (3,3) and 64 filters.
     - Max pooling layer to improve feature mapping and reduce data size.
  2. The output layer utilized a **linear** activation function with 10 unit for classification and then later **softmax** was used to predict the probabilities of each outcomes and then pick the best one with argmax and predict that outcomes

- **Performance**:
  - The model achieved the following metrics:
  - accuracy: 88 
  - loss: 0.3430
  - val_accuracy: 65.88
  - val_loss: 1.2737

This implementation demonstrates effective classification of cats and dogs using Convolutional Neural Networks.
