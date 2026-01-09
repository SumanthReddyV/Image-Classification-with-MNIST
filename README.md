# Image-Classification-with-MNIST

This repository contains a "Hello World" project for Deep Learning: training a neural network to classify handwritten digits using the MNIST dataset. The project is implemented using PyTorch 2.0 and the Sequential API.

## 🚀 Project Objectives
The goal of this notebook is to demonstrate a complete machine learning workflow, including:

- **Data Engineering**: Loading and preparing 70,000 grayscale images for training and validation.
- **Tensor Manipulation**: Converting images to tensors and managing GPU acceleration via CUDA.
- **Model Construction**: Building a multi-layer neural network with input, hidden, and output layers.
- **Training & Evaluation**: Implementing a training loop with loss functions and optimizers to reach high accuracy.

## 🛠️ Model Architecture
The model is built using `torch.nn.Sequential` and consists of the following architecture:

- **Flatten Layer**: Converts the $1 \times 28 \times 28$ image tensor into a 1D vector of 784 pixels.
- **Input Layer**: A fully connected (Linear) layer with 512 neurons and ReLU activation.
- **Hidden Layer**: A second dense layer with 512 neurons and ReLU activation to capture complex patterns.
- **Output Layer**: A final linear layer with 10 neurons, representing the digits 0-9.

## 📈 Performance
The model was trained for 5 epochs using the Adam optimizer and CrossEntropyLoss.

- **Training Results**: Achieved near 100% accuracy on the training set.
- **Validation Results**: Successfully maintained high accuracy on unseen data, proving the model's ability to generalize.