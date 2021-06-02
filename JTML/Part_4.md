[Previous](https://github.com/BRIO-lab/brio-lab-onboarding/blob/main/JTML/Part_3.md) | [Next](https://github.com/BRIO-lab/brio-lab-onboarding/blob/main/JTML/Part_5.md)

# JTML Part 4: Machine Learning and Neural Networks

Machine learning and "big data" has become very common in modern research. With new computational power and the introduction of the [Graphics Processing Unit](https://en.wikipedia.org/wiki/Graphics_processing_unit), researchers have been able to make tremendous strides toward solving computationally expensive problems. One of the main benefits of these types of approaches is that they can eliminate the need for human supervision for many different tasks, including, but not limited to: playiong chess, categorizing images, recognizing speech, identifying dog types, and labeling pixels in images.

There are a few different resources that are extremely useful to get caught up in machine learning. They will take your from the very beginning to neural networks.

In Depth Classes/Resources:

[Andrew Ng Machine Learning Coursera Course](https://www.coursera.org/learn/machine-learning)

[Andrew Ng Deep Learning Courserea Course](https://www.coursera.org/specializations/deep-learning)

[Stanford CS231n - Convolutional Neural Networks for Image Recognition](https://youtube.com/playlist?list=PLC1qU-LWwrF64f4QKQT-Vg5Wr4qEE1Zxk)

Quicker Reads:

[A Comprehensive Guide to Convolutional Neural Networks — the ELI5 way](https://towardsdatascience.com/a-comprehensive-guide-to-convolutional-neural-networks-the-eli5-way-3bd2b1164a53)


If you watch and participate in these, you will have a very strong grasp of the machine learning that we are doing in this lab.

## What are we using machine learning for?

Remember those limitations that we encountered with model-image registration from the previous page? We are trying to use machine learning to combat those limitations. We utilize a 2-fold approach to machine learning.

1. Segmentation
    * We use segmentation to label the pixels of the images that we are looking at as either (a) region of interest or (b) not region of interest. This usually means that we are labeling an implant or a bone.
    * This overcomes the issues of implant occlusion and other problems while creating a segmentation.
2. Pose Estimation
    * From the segmented image, we are estimating the pose using a neural network, providing and initial guess for the optimizer to run.
    * This overcomes the issue of needing human supervision during the optimization process.

## Some Machine Learning Papers and Books

[Krizhevsky et al - 2017 - ImageNet Classification with Deep Convolutional Neural Networks](https://www.dropbox.com/s/ugcd5lwrzdx400j/Krizhevsky%20et%20al_2017_ImageNet%20classification%20with%20deep%20convolutional%20neural%20networks.pdf?dl=0)

[Goodfellow - 2016 - Deep Learning Book](https://www.deeplearningbook.org/)

## Some Useful Resources in General

[Papers with Code]() - this is a really great resource that consolidates the academic journals that included the code they used to generate the results.

[Sentdex - Deep Learning with Python (PyTorch)](https://youtube.com/playlist?list=PLQVvvaa0QuDdeMyHEYc0gxFpYwHY2Qfdh) - shows how to use PyTorch in a pretty basic way to understand the general syntax of the library. This is the library that we will be using for our code.

[Sentdex - Neural Networks from Scratch in Python](https://youtube.com/playlist?list=PLQVvvaa0QuDcjD5BAw2DxE6OF2tius3V3) - a few videos that explain very simply the basic structure of a neural network. Pretty straightforward, and you learn how some of the components are implemented in code.


[Previous](https://github.com/BRIO-lab/brio-lab-onboarding/blob/main/JTML/Part_3.md) | [Next](https://github.com/BRIO-lab/brio-lab-onboarding/blob/main/JTML/Part_5.md)