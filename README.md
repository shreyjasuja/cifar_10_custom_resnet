# CIFAR-10 classification using Custom Resnet
-Mini Project for ECE- GY  7123

This is an implementation of residual learning and shortcut connections for deep neural networks, based on the paper "Deep Residual Learning for Image Recognition" by Kaiming He et al..

## Introduction
Residual Networks (ResNets) were developed to address the vanishing gradient problem by introducing residual blocks, and subsequent research by Hao Li et al. (2018) has shown that skip connections make the loss landscape smoother. ResNets enable training of very deep networks, which was not possible before. In this study, we explore custom ResNet architectures for classifying the CIFAR-10 image dataset. CIFAR-10 is a small dataset with 10 classes, making it a suitable testbed for evaluating design choices. We performed approximately 15 experiments, varying the number of layers, filters, dropout rates, and learning rate schedulers.

## Implementation
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shreyjasuja/cifar_10_custom_resnet/blob/main/dl_mini_project.ipynb)

The implementation is based on the PyTorch deep learning framework. The [Custom Resnet](dl_mini_project.ipynb) jupyter file contains the ResNet implementation, which can be used to train and evaluate deep neural networks for image recognition tasks.
<br />
Model weights are available [here](https://bit.ly/dl-7123)

## Results
![loss metrics](https://drive.google.com/uc?export=view&id=1RABEx5c5jyCaGhxsOfx6wi48nnE1Do7h)

The trained ResNet model on the CIFAR-10 test gave the accuracy of **95.16 %**.

## Credits
This implementation was created by Shrey Jasuja, Prasanna Sai Puvvada, Rahul Raj based on the ResNet paper by Kaiming He et al. The PyTorch framework was used for the implementation.

## License
This project is licensed under the GNU License - see the [LICENSE](LICENSE) file for details.





