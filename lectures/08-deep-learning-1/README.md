# Lecture 08: Deep Learning - I

**Instructor:** Yash  
**Date:** May 25, 2025

---

## 📖 Overview

This lecture served as an introduction to deep learning. We covered the foundational concepts and intuition behind how neural networks learn from data. Topics included:

- Types of data-driven learning: **supervised**, **unsupervised**, and **self-supervised** learning
- The **perceptron** as a basic computational unit
- **Forward propagation**, **gradient calculation**, and **optimization using gradient descent**
- Training a simple neural network for **MNIST digit classification**, demonstrated through [`mnist.ipynb`](./mnist.ipynb)


---

## 📄 Assignment
> The following section was contributed by **Yash** — credit to him for this neat instructive hands-on.

First unzip `mnist.pkl.zip` to get the `mnist.pkl` file. This file contains the MNIST dataset, which is a collection of 70,000 handwritten digits (0-9) used for training and testing machine learning models.

Use the following snippet to load the mnist data
```py
def load()
    with open("mnist.pkl",'rb') as f:
        mnist = pickle.load(f)
    return mnist["training_images"], mnist["training_labels"], mnist["test_images"], mnist["test_labels"]
```
In your code if you run:

```py
x_train, t_train, x_test, t_test = load()
```

This would return 4 numpy arrays:
- x_train : 60,000x784 numpy array that each row contains flattened version of training images.
- t_train : 1x60,000 numpy array that each component is true label of the corresponding training images.
- x_test : 10,000x784 numpy array that each row contains flattened version of test images.
- t_test : 1x10,000 numpy array that each component is true label of the corresponding test images.


Keep in mind that all it takes for one layer is:
- one matrix multiplication (the weights)
- one bias vector for the layer (the bias)
- an activation

You can make a network as follows, although I encourage you to experiment different number of layers, and different sizes of layers. 
1. The Input Layer: 784 neurons (because 28x28 = 784)
2. The Hidden Layer will take in the fed-forward 784 datapoints into it’s 32 neurons and output 32 values.
3. The Output Layer will take in the 32 output values from the hidden layer into it’s 10 neurons and output 10 activation values, of which the neuron with the highest activation value will correspond to the networks final digit prediction.

You can use ReLU as the activation, Gradient descent as the optimization. Experiment with the step size. Try some comically high step size (~0.2) or some comically low step size (1e-6), and the Categorical Cross Entropy Loss, and the backprop. 

```py
def cat_cross_entropy(one_hot_Y, network_output):
    CCE = -np.sum(one_hot_Y * np.log(network_output)) * 1/m
    return CCE
 ```
Where `m` is equal to the total number of samples (digits) in our dataset.
You would need to define a few functions for ReLU, for Softmax, for making the labels one-hot (recall why we discussed making them one hot is important)

Feel free to look up for help online (coding up a network for MNIST is quite a widely accepted exercise for practice for beginners, and was incredibly rewarding when I coded mine), or reach out on Slack (**`#module-3-deep-learning`**).

Happy Learning!

---

## 🔗 Resources

| Topic                                  | Link                                                                                                       |
|---------------------------------------|------------------------------------------------------------------------------------------------------------|
| Lecture Slides - Deep Learning Basics | [lec-08-dl-basics.pdf](./lec-08-dl-basics.pdf)                                                             |
| MNIST Classification Demo              | [mnist.ipynb](./mnist.ipynb)                                                                             |
| 3Blue1Brown – Deep Learning Playlist  | [YouTube: 3b1b Neural Networks](https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi)  |
| Andrew Ng – Deep Learning Specialization | [Coursera: DeepLearning.AI](https://www.coursera.org/specializations/deep-learning)                      |
| DeepLizard – YouTube Channel          | [YouTube: DeepLizard](https://www.youtube.com/c/deeplizard)                                                |
| Deep Learning – Ian Goodfellow et al. | [Book: Deep Learning (Goodfellow)](https://www.deeplearningbook.org/)                                     |
| Mathematics for Machine Learning – A. Faisal et al. | [Book: Mathematics for Machine Learning](https://mml-book.github.io/)                              |
| Dive into Deep Learning – Aston Zhang et al. | [Book: Dive into Deep Learning (d2l.ai)](https://d2l.ai/) |

---
