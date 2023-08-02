# Udacity project Face Generator using CelebA
This project was part of the [Udacity Deep Learning Nano Degree Program](https://www.udacity.com/course/deep-learning-nanodegree--nd101) 
that was teaching basics on building Generative Adversarial Networks (GANs).

In this project, we did build and train a custom GAN architecture on the CelebA dataset, 
leveraging the different skills learned during the course mentioned above.

## Model Architecture
### Deep Convolutional GANs
In this notebook, I've chosen to apply the DCGAN architecture to build a GAN using convolutional layers in the generator and discriminator. 
This is called a Deep Convolutional GAN, or DCGAN for short. 

The DCGAN architecture was first explored in 2016 and has seen impressive results in generating new images. 
You can read the original paper, [here](https://arxiv.org/pdf/1511.06434.pdf).

Next to using Convolutional layers, I used label smoothing technique for the discriminator and the
'Two Times Update Rule' for the genrator part of the model.  

## Data Set
You’ll be training DCGAN on the [Large-scale CelebFaces Attributes (CelebA) Dataset](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) dataset. 

These are color images of celebrities. In this course, Udacity provides a smaller subset of this data set with in total 32,600 pre-processed images.
More details are provided by Udacity in the Jupyter notebook `face_generator.ipynb`.

# Getting Started
So, our goal is to create a DCGAN that can generate new, realistic-looking images. 
We’ll go through the following steps:
1. Extract the prepared subset of the celeb data set
2. Define discriminator and generator networks
3. Train the DCGAN network
4. Visualize the loss over time and some sample, generated images

## Requirements
It is recommended to train the model on GPU.
