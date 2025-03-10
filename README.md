# GoogLeNet Architecture
GoogLeNet is a type of convolutional neural network based on the Inception architecture. It utilises Inception modules, which allow the network to choose between multiple convolutional filter sizes in each block. An Inception network stacks these modules on top of each other, with occasional max-pooling layers with stride 2 to halve the resolution of the grid.
GoogLeNet (Inception v1) is a pioneering deep convolutional neural network architecture known for its efficiency and performance in image classification tasks. Here are its pros and cons:
Pros:
####Computational Efficiency: Uses 1x1 convolutions to reduce the number of parameters and computational cost, making it more efficient than deeper networks like VGG.

####Inception Modules: Employs parallel convolutional operations with multiple filter sizes (1x1, 3x3, 5x5) and pooling layers, enabling the network to capture features at different scales simultaneously.

####Deeper Network with Fewer Parameters: Despite being 22 layers deep, GoogLeNet has significantly fewer parameters compared to VGG-16 or VGG-19, reducing the risk of overfitting.

####Auxiliary Classifiers: Introduces auxiliary classifiers during training to combat the vanishing gradient problem and improve gradient flow in deeper layers.

####High Performance: Achieved state-of-the-art results on the ImageNet Large Scale Visual Recognition Challenge (ILSVRC) in 2014 with a top-5 error rate of 6.67%.

####Scalability: The Inception module design is modular and scalable, forming the basis for later versions like Inception v2, v3, and v4.


### Inception Module : 
An Inception module is a key component of the Inception architecture in convolutional neural networks (CNNs). It is designed to efficiently extract features at multiple scales by applying parallel convolutional operations with varying filter sizes (e.g., 1x1, 3x3, 5x5) and pooling layers within the same module. These parallel operations are concatenated, allowing the network to capture both fine-grained and coarse-grained features simultaneously. The use of 1x1 convolutions reduces computational complexity, making the module computationally efficient while maintaining high performance in tasks like image classification and object detection.

![Inception Module](https://github.com/user-attachments/assets/14371a02-9d29-4f2f-9ac1-4c311f69517e)
