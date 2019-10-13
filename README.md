# CNN-Visualized
## How to read the images 
- [ ] TODO explain how the design works 
# Template
## [Title]()
*Authors*

Lorem Ipsum (fast description)

![alt](https://kharshit.github.io/img/resnet_50.png)

## [Alexnet](https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf)
*Alex Krizhevsky, Ilya Sutskever, 
Geoffrey E. Hinton* - 2010

Alexnet started the deep learning revolution, it is a very simple model composed by convolution/relu block followed by three big fully connected layers. 


![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/develop/images/alexnet/AlexNet.png?raw=true)

Where each colored block (conv block) are convolution followed by a **ReLU**

![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/develop/images/alexnet/AlexNetConv.png?raw=true)

And each white blocks are just fully connected layer followed by a **ReLU**

![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/develop/images/alexnet/AlexNetFC.png?raw=true)

## [ResNet](https://arxiv.org/abs/1512.03385)
ResNet introduced residual connection in which the input to a block is added to its ouput to boost gradient flow throught the model. They defined two diffent block and stack them together to create different architectures. 

### ResNet18
![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/develop/images/resnet/ResNet18.png?raw=true)

#### BasicBlock
Each basic block is composed by two conv 3x3 with relu and batchnorm
![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/develop/images/resnet/ResNetBasicBlock.png?raw=true)
#### Residual Connection
When the input of a basic block have not the same features of the output of a block, we need downsampling to match the correct features size. This is done in the dotted line by using another conv 1x1 layer.
![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/develop/images/resnet/ResNetDownSampling.png?raw=true)
### ResNet34
![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/develop/images/resnet/ResNet34.png?raw=true)
### ResNet50
![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/develop/images/resnet/ResNet50.png?raw=true)
#### BottleNeck Block
To reduce the computation footprint, the bottleneck fist reduce the features of the input using a 1x1, apply the expensive 3x3 and then rematch the previous size with another 1x1
![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/develop/images/resnet/ResNetBottleNeck.png?raw=true)
### ResNet101
![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/develop/images/resnet/ResNet101.png?raw=true)
### ResNet152
![alt](https://github.com/DeepLearningPoets/CNN-Visualized/blob/develop/images/resnet/ResNet152.png?raw=true)

# TODO
List of models to draw

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
