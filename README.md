# Arrhythmia Detection

This repository contains the implementation of a neural network for detecting arrhythmia using the dataset from [Kaggle](https://www.kaggle.com/datasets/shayanfazeli/heartbeat).

## 1. Model Architecture

![Model Architecture](https://github.com/umang4002/Arrythmiya/blob/main/network_new%20(1).png)

The model architecture is designed to efficiently classify heartbeat signals into different classes, leveraging a combination of convolutional and residual blocks.

## 2. Residual Inverted Convolution (RIC) Block

![RIC Block](https://github.com/umang4002/Arrythmiya/blob/main/RIC_best%20(1).png)

The Residual Inverted Convolution (RIC) Block is a key component of the network, enhancing feature extraction through residual connections and inverted convolutions.

## 3. Results

The model has a total of 19.6K parameters. The performance metrics for each class are as follows:

| Class   | Precision | Recall | Specificity | NPV   | Accuracy |
|---------|-----------|--------|-------------|-------|----------|
| Class 0 | 0.9887    | 0.9966 | 0.9452      | 0.9829| 0.9877   |
| Class 1 | 0.9161    | 0.7464 | 0.9982      | 0.9934| 0.9918   |
| Class 2 | 0.9666    | 0.9606 | 0.9977      | 0.9972| 0.9952   |
| Class 3 | 0.8897    | 0.7469 | 0.9993      | 0.9981| 0.9974   |
| Class 4 | 0.9925    | 0.9882 | 0.9994      | 0.9991| 0.9986   |

### Definitions:
- **Precision**: The ratio of true positive predictions to the total predicted positives.
- **Recall**: The ratio of true positive predictions to the total actual positives.
- **Specificity**: The ratio of true negative predictions to the total actual negatives.
- **NPV (Negative Predictive Value)**: The ratio of true negative predictions to the total predicted negatives.
- **Accuracy**: The ratio of correct predictions (both true positives and true negatives) to the total predictions.

## Dataset

The dataset used in this project can be found on Kaggle: [Heartbeat Dataset](https://www.kaggle.com/datasets/shayanfazeli/heartbeat).


## 4. References

Li, Duo, et al. "Involution: Inverting the inherence of convolution for visual recognition." Proceedings of the IEEE/CVF conference on computer vision and pattern recognition. 2021.
