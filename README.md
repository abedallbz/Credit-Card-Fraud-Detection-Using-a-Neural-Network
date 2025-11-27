Project Overview

The goal is to classify each transaction as:

0 → Legitimate

1 → Fraudulent

The notebook uses a neural network with several layers, trained directly on transaction features. It also includes exploratory ideas on detecting fraud based on user behavior and transaction patterns.

🧠 🧩 Methods & Architecture
✔ 1. Manual Implementation of Deep Neural Network

The notebook includes complete implementations of:

Parameter initialization
initialize_parameters()

Linear forward step
linear_forward(A_prev, W, b)

Activation functions

Sigmoid

ReLU
using
sigmoid(Z) and relu(Z)

Forward propagation for one layer
linear_activation_forward(A_prev, W, b, activation)

Multi-layer forward propagation
L_model_forward(X, parameters)

Cost computation
Using binary cross-entropy

Backward propagation
Linear + activation derivatives
linear_backward, relu_backward, sigmoid_backward

Full backprop for L-layer model
L_model_backward(AL, Y, caches)

Gradient descent parameter update
update_parameters(parameters, grads, learning_rate)

This makes the project ideal for educational purposes and transparency.

📊 2. Dataset Handling

Data loaded from CSV (Kaggle credit card fraud dataset)

Features include:

Time

V1–V28 (PCA-transformed financial features)

Amount

Preprocessing includes scaling and reshaping features into neural-network-ready form

🏗 3. Neural Network Structure

Although the architecture is customizable, typical structure used:

Input layer  → Hidden layer(s) (ReLU) → Output layer (Sigmoid)


Examples:

[30 → 20 → 7 → 5 → 1]

Or simpler variants

You control the architecture by choosing the number and size of layers.

🎯 4. Training

The notebook:

Runs forward propagation

Computes the loss

Runs backward propagation

Updates parameters using gradient descent

Repeats for multiple epochs until convergence

📈 5. Evaluation

The model outputs:

Accuracy

Number of fraud examples correctly predicted

False positives / false negatives

Performance visualization using Matplotlib

🔐 6. Fraud-Detection Considerations

The notebook also includes discussion ideas, such as:

Location-based fraud detection

Time-based fraud anomalies

User behavior patterns

Multi-fraud classification

Transaction frequency analysis

These serve as future extensions and documentation notes inside the notebook.

🧰 Technologies Used

Python

NumPy

Pandas

Matplotlib

Basic machine learning

Custom-written neural network code

🎯 Purpose of This Project

This notebook is ideal for:

Learning how to build a neural network from scratch

Understanding fraud detection techniques

Demonstrating ML concepts in a transparent way

Practicing manual backpropagation and deep learning fundamentals
