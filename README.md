# Siamese Network

[![GitHub stars](https://img.shields.io/github/stars/elcaiseri/Siamese-Network)](https://github.com/elcaiseri/Siamese-Network/stargazers)
[![GitHub watchers](https://img.shields.io/github/watchers/elcaiseri/Siamese-Network)](https://github.com/elcaiseri/Siamese-Network/watchers)

This repository contains an example of using a Siamese Network with a triplet loss for image similarity estimation. A [Siamese Network](https://en.wikipedia.org/wiki/Siamese_neural_network) is a type of network architecture that
contains two or more identical subnetworks used to generate feature vectors for each input and compare them.

Siamese Networks can be applied to different use cases, like detecting duplicates, finding anomalies, and face recognition.

This example uses a Siamese Network with three identical subnetworks. We will provide three images to the model, where
two of them will be similar (_anchor_ and _positive_ samples), and the third will be unrelated (a _negative_ example.)
Our goal is for the model to learn to estimate the similarity between images.

For the network to learn, we use a triplet loss function. You can find an introduction to triplet loss in the
[FaceNet paper](https://arxiv.org/pdf/1503.03832.pdf) by Schroff et al,. 2015.

Siamese Networks can be applied to various use cases, such as detecting duplicates, finding anomalies, and face recognition.

## Table of Contents
- [Introduction](#introduction)
- [Setup](#setup)
- [Load the Dataset](#load-the-dataset)
- [Preparing the Data](#preparing-the-data)
- [Setting up the Embedding Generator Model](#setting-up-the-embedding-generator-model)
- [Setting up the Siamese Network Model](#setting-up-the-siamese-network-model)
- [Putting Everything Together](#putting-everything-together)
- [Training](#training)
- [Inspecting What the Network Has Learned](#inspecting-what-the-network-has-learned)
- [Summary](#summary)
- [About](#about)

## Introduction
A Siamese Network with a triplet loss function is used in this example to estimate the similarity between images. The triplet loss function is defined as follows:

```
L(A, P, N) = max(‖f(A) - f(P)‖² - ‖f(A) - f(N)‖² + margin, 0)
```

## Setup
This example uses the Totally Looks Like dataset by Rosenfeld et al., 2018.

## Load the Dataset
The dataset used in this example is named "Totally Looks Like." It contains images to create triplets (anchor, positive sample, and negative sample) for training.

## Preparing the Data
Prepare the data for training the Siamese Network by creating triplets of images.

## Setting up the Embedding Generator Model
Create a model that generates embeddings for each image in a triplet.

## Setting up the Siamese Network Model
Construct the Siamese Network model using three identical subnetworks.

## Putting Everything Together
Combine all the components to form the complete Siamese Network.

## Training
Train the Siamese Network using the triplet loss function.

## Inspecting What the Network Has Learned
Evaluate the network's performance and inspect the embeddings learned by the model.

## Summary
A summary of the key points covered in the example.

## About
This example demonstrates image similarity estimation using a Siamese Network with a triplet loss.

© 2023 [elcaiseri](https://github.com/elcaiseri)

---
*GitHub is not affiliated with this project. The names and logos mentioned above are trademarks of their respective owners.*
