# GoogLeNet Architecture
GoogLeNet is a type of convolutional neural network based on the Inception architecture. It utilises Inception modules, which allow the network to choose between multiple convolutional filter sizes in each block. An Inception network stacks these modules on top of each other, with occasional max-pooling layers with stride 2 to halve the resolution of the grid.


### Inception Module : 
An Inception module is a key component of the Inception architecture in convolutional neural networks (CNNs). It is designed to efficiently extract features at multiple scales by applying parallel convolutional operations with varying filter sizes (e.g., 1x1, 3x3, 5x5) and pooling layers within the same module. These parallel operations are concatenated, allowing the network to capture both fine-grained and coarse-grained features simultaneously. The use of 1x1 convolutions reduces computational complexity, making the module computationally efficient while maintaining high performance in tasks like image classification and object detection.

![Inception Module](https://github.com/user-attachments/assets/14371a02-9d29-4f2f-9ac1-4c311f69517e)


### Architecture : 
In this architecture, we tried to implement all the goals in a modular way. In this architecture, we need to be able to move around the image and identify objects and points, given the kernel-size, padding, and stride.
