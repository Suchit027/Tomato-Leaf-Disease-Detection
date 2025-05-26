# Tomato-Leaf-Disease-Detection

## Overview
The aim of this project is to detect what kind of disease does the tomato has from the images of its leaves. The project accomplishes this task with the help of CNN and ResNets.

## Methodology
First features are extracted using ResNet 50. The extracted features are passed into a custom CNN model. This model analyzes the extracted features and finds more meaningfull and output determining features.<br>
The CNN model includes 5 Conv2d layers. After each layer, batch norm is applied to normalize the outputs. ReLU activation function is used.<br>
Dropout layer with dropout probability of 0.2 is used for creating an ensemble of networks. <br>
Cross Entropy Loss is used. AdamW optimizer is used instead of Adam for better regularization and less impact on adaptive learning rates.<br>
ReduceLROnPlateau learning rate scheduler is used to reduce the learning rate when the training stagnates.<br>
The results are compared with Random Forest algorithm. Both give the same accuracy.
