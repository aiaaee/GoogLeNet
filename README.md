# [GoogLeNet Architecture](https://github.com/aiaaee/GoogLeNet/blob/main/GoogLeNet.ipynb) 
GoogLeNet is a type of convolutional neural network based on the Inception architecture. It utilises Inception modules, which allow the network to choose between multiple convolutional filter sizes in each block. An Inception network stacks these modules on top of each other, with occasional max-pooling layers with stride 2 to halve the resolution of the grid.
The Inception Network was one of the major breakthroughs in the fields of Neural Networks, particularly for CNNs. So far there are three versions of Inception Networks, which are named Inception Version 1, 2, and 3. The first version entered the field in 2014, and as the name “GoogleNet” suggests, it was developed by a team at Google. This network was responsible for setting a new state-of-the-art for classification and detection in the ILSVRC. This first version of the Inception network is referred to as GoogleNet.



### Inception Module : 
An Inception module is a key component of the Inception architecture in convolutional neural networks (CNNs). It is designed to efficiently extract features at multiple scales by applying parallel convolutional operations with varying filter sizes (e.g., 1x1, 3x3, 5x5) and pooling layers within the same module. These parallel operations are concatenated, allowing the network to capture both fine-grained and coarse-grained features simultaneously. The use of 1x1 convolutions reduces computational complexity, making the module computationally efficient while maintaining high performance in tasks like image classification and object detection.

![Inception Module](https://github.com/user-attachments/assets/14371a02-9d29-4f2f-9ac1-4c311f69517e)


### Architecture : 
In this architecture, we tried to implement all the goals in a modular way. In this architecture, we need to be able to move around the image and identify objects and points, given the kernel-size, padding, and stride.  The architecture was designed to keep computational efficiency in mind. The idea behind that the architecture can be run on individual devices even with low computational resources. The architecture also contains two auxiliary classifier layer connected to the output of Inception (4a) and Inception (4d) layers.

![Inceptionv1_architecture](https://github.com/user-attachments/assets/e917a352-df28-47f4-9752-cf71ff1295a0)



### GoogleNet Training and Results
GoogleNet is trained using distributed machine learning systems with a modest amount of model and data parallelism. The training used asynchronous stochastic gradient descent with a momentum of 0.9 and a fixed learning rate schedule decreasing the learning rate by 4% every 8 epochs. Below is an image of the results of the teams that performed for ILSVRC 2014. GoogleNet stood in first place with an error rate of 6.67%.


