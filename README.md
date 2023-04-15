# CIFAR-10 classification using Custom Resnet
-Mini Project for ECE- GY  7123


This is an implementation of residual learning and shortcut connections for deep neural networks, based on the paper "Deep Residual Learning for Image Recognition" by Kaiming He et al..

##Introduction
Residual Networks (ResNets) were developed to address the vanishing gradient problem by introducing residual blocks, and subsequent research by Hao Li et al. (2018) has shown that skip connections make the loss landscape smoother. ResNets enable training of very deep networks, which was not possible before. In this study, we explore custom ResNet architectures for classifying the CIFAR-10 image dataset. CIFAR-10 is a small dataset with 10 classes, making it a suitable testbed for evaluating design choices. We performed approximately 15 experiments, varying the number of layers, filters, dropout rates, and learning rate schedulers.

In residual learning, we let the stacked layers directly fit the required underlying mapping, and also fit a residual mapping. This allows us to recast the original mapping to $F(x) + x$, where $F(x)$ is a block that implements convolution, batch normalization, and ReLU activation. The original mapping is then simpler to optimize than the original, unreferenced mapping.

Shortcut connections that skip one or more layers are also used to implement the formulation of $F(x) + x$. In this implementation, the shortcut connections carry out identity mapping, and their results are added to those of the stacked layers.

##Implementation
The implementation is based on the PyTorch deep learning framework. The ![Custom Resnet](dl_mini_project.ipynb) file contains the ResNet implementation, which can be used to train and evaluate deep neural networks for image recognition tasks.




The trained ResNet model on the CIFAR-10 test gave the accuracy of **95.16 %**.

##Credits
This implementation was created by Shrey Jasuja, Prasanna Sai Puvvada, Rahul Raj based on the ResNet paper by Kaiming He et al. The PyTorch framework was used for the implementation.

##License
This project is licensed under the GNU License - see the ![LICENSE](LICENSE) file for details.





