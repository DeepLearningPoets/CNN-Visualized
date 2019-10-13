# CNN-Visualized
## How to read the images 
We used [figma](www.figma.com) to create all the networks. Each rectangle represent an operation, for example.
- [ ] TODO explain how the design works 
# Legend

# Template
## [Title]()
*Authors*

Lorem Ipsum (fast description)

![alt](https://kharshit.github.io/img/resnet_50.png)

## [Alexnet](https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf)
*Alex Krizhevsky, Ilya Sutskever, 
Geoffrey E. Hinton* - 2010

Alexnet started the deep learning revolution, it is a very simple model composed by **convolution** and **relu** blocks followed by three big **fully connected** layers. 

![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/develop/images/alexnet/AlexNet.png?raw=true)

Where each colored block (conv block) are convolution followed by a **ReLU**

![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/develop/images/alexnet/AlexNetConv.png?raw=true)

And each white blocks are just fully connected layer followed by a **ReLU**

![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/develop/images/alexnet/AlexNetFC.png?raw=true)


## [U-Net](https://arxiv.org/abs/1512.03385)
*Olaf Ronneberger, Philipp Fischer, Thomas Brox* - 2015
![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/develop/images/unet/UNet.png?raw=true)

## [ResNet](https://arxiv.org/abs/1512.03385)
*Kaiming He, Xiangyu Zhang, Shaoqing Ren, Jian Sun* - 2015

ResNet introduced residual connection in which the input to a block is added to its ouput to boost gradient flow throught the model. They defined two diffent block and stack them together to create different architectures. 

### ResNet18
![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/develop/images/resnet/ResNet18.png?raw=true)

#### BasicBlock
Each *BasicBlock** is composed by two conv 3x3 with relu and batchnorm
![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/develop/images/resnet/ResNetBasicBlock.png?raw=true)
#### Residual Connection
When the input of a basic block have not the same features of the output of a block, we need downsampling to match the correct features size. This is done in the dotted line by using another conv 1x1 layer.
![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/develop/images/resnet/ResNetDownSampling.png?raw=true)
### ResNet34
![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/develop/images/resnet/ResNet34.png?raw=true)
### ResNet50
![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/develop/images/resnet/ResNet50.png?raw=true)
#### BottleNeck Block
To reduce the computation footprint, the *BottleNeck* block fist reduce the features of the input using a 1x1, apply the expensive 3x3 and then rematch the previous size with another 1x1
![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/develop/images/resnet/ResNetBottleNeck.png?raw=true)
### ResNet101
![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/develop/images/resnet/ResNet101.png?raw=true)
### ResNet152
![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/develop/images/resnet/ResNet152.png?raw=true)


## [Inception](https://arxiv.org/pdf/1602.07261)
Inception denotes a class of heavily hand-engineered architectures, of which GoogLeNet network was the first example, designed to improve the utilization of computing resources, while getting both the benefit from having small and large convolutional kernels. Since the first release, there have been a progression of improvements on the architecture:
- [Inception v1](https://arxiv.org/abs/1409.4842)
- [Inception v2 and v3](https://arxiv.org/pdf/1512.00567v3)
- [Inception v4 and Inception ResNet](https://arxiv.org/pdf/1602.07261)

In what follows, we propose the Inception v4 architecture.

### Inception-v4 modules
The Inception-v4 network is built on six different modules: stem, inception modules A, B and C and reduction modules A and B.
![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/master/images/inception/Inception.png?raw=true)

#### Filters Concatenation
Inception modules make a heavy use of filters concatenation, which we represented here with two squared brackets *[ ]*. In this process, filters generated from different convolutional kernels are concatenated and forwarded together. 

#### Stem Module
The stem module applies some preliminary convolutions.
![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/master/images/inception/InceptionStem.png?raw=true)

#### Inception-A
![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/master/images/inception/InceptionA.png?raw=true)

#### Inception-B
![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/master/images/inception/InceptionB.png?raw=true)

#### Inception-C
![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/master/images/inception/InceptionC.png?raw=true)

#### Reduction-A
![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/master/images/inception/ReductionA.png?raw=true)

#### Reduction-B
![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/master/images/inception/ReductionB.png?raw=true)



# TODO
List of models to draw

- [x] [alexnet](https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf) - 2010
- [ ] [vgg](https://arxiv.org/pdf/1409.1556.pdf) - 15 apr 2015
- [x] [inception](https://arxiv.org/pdf/1409.4842.pdf) - 17 sept 2014
- [x] [U-Net](https://arxiv.org/abs/1505.04597) - 18 May 2015
- [x] [resnet](https://arxiv.org/abs/1512.03385)10 Dec 2015
- [ ] [resnet - preactivation](https://arxiv.org/abs/1603.05027)- 16 Mar 2016 
- [ ] [FractalNet](https://arxiv.org/abs/1605.07648) - 24 May 2016
- [ ] [ResNeXt](https://arxiv.org/abs/1611.05431) - 16 Nov 2016
- [ ] [PolyNet](https://arxiv.org/abs/1611.05725) - 17 Nov 2016
- [ ] [densenet](https://arxiv.org/abs/1608.06993) - 25 Aug 2016
- [ ] [squeeze and excitation/SENet](https://arxiv.org/abs/1709.01507) - 5 Sep 2017
- [ ] [LegoNet](http://proceedings.mlr.press/v97/yang19c/yang19c.pdf) - 2019
- [ ] [EfficientNet](https://arxiv.org/abs/1905.11946) - 10 jun 2019

List of models to write

- [ ] [alexnet](https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf) - 2010
- [ ] [vgg](https://arxiv.org/pdf/1409.1556.pdf) - 15 apr 2015
- [ ] [inception](https://arxiv.org/pdf/1409.4842.pdf) - 17 sept 2014
- [ ] [U-Net](https://arxiv.org/abs/1505.04597) - 18 May 2015
- [ ] [resnet](https://arxiv.org/abs/1512.03385)10 Dec 2015
- [ ] [resnet - preactivation](https://arxiv.org/abs/1603.05027)- 16 Mar 2016 
- [ ] [FractalNet](https://arxiv.org/abs/1605.07648) - 24 May 2016
- [ ] [ResNeXt](https://arxiv.org/abs/1611.05431) - 16 Nov 2016
- [ ] [PolyNet](https://arxiv.org/abs/1611.05725) - 17 Nov 2016
- [ ] [densenet](https://arxiv.org/abs/1608.06993) - 25 Aug 2016
- [ ] [squeeze and excitation/SENet](https://arxiv.org/abs/1709.01507) - 5 Sep 2017
- [ ] [LegoNet](http://proceedings.mlr.press/v97/yang19c/yang19c.pdf) - 2019
- [ ] [EfficientNet](https://arxiv.org/abs/1905.11946) - 10 jun 2019