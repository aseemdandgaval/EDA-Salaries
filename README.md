# EDA-Salaries

This project is an Exploratory Data Analysis on the salaries of preofessionals working in the data domain in India.

https://github.com/aseemdandgaval/EDA-Salaries/blob/main/EDA_Industy_Salaries.ipynb <br />
(Check this notebook for a slightly in-depth explaination and the code.) 

<br>

## The Dataset

Generative Adversarial Networks or GANs , are used for Generative modeling.
Generative modeling is an unsupervised learning task in machine learning that involves automatically discovering and learning the regularities or patterns in input data in such a way that the model can be used to generate or output new examples that plausibly could have been drawn from the original dataset.

## Model and Training

<img src="https://i.imgur.com/6NMdO9u.png" style="width:300px; margin-bottom:32px"/>

There are two neural networks: a **Generator** and a **Discriminator**. The generator generates a "fake" sample given a random vector/matrix, and the discriminator attempts to detect whether a given sample is "real" (picked from the training data) or "fake" (generated by the generator).
Training happens in tandem: we train the discriminator for a few epochs, then train the generator for a few epochs, and repeat. This way both the generator and the discriminator get better at doing their jobs. 

GANs however, can be notoriously difficult to train, and are extremely sensitive to hyperparameters, activation functions and regularization. 

## Dataset

![image](https://user-images.githubusercontent.com/79587733/149305253-72031e4d-f1b8-4296-8d4b-78eb920bb45d.png)

I have used the [Abstract Art Gallery](https://www.kaggle.com/muhammad4hmed/gan-aa/data) dataset which consists of 2800 images of abstract images.

## Discriminator Network

The discriminator takes a `3 x 512 x 512` image as input, and tries to classify it as "real" or "generated/fake". The discriminator is a simple Convolutional Neural Network (CNN) which does binary classification, with **0** and **1** as its outputs signifying a **fake** or a **real** image respectively.

![image](https://user-images.githubusercontent.com/79587733/149306230-281a1cde-155b-49cf-9a49-2bb9ac9d4dbe.png)

## Generator Network

The input to the generator is typically a vector or a matrix of random numbers, referred to as a **latent tensor** which is used as a seed for generating an image. The generator will convert a latent tensor of shape `(256, 1, 1)` into an image tensor of shape `3 x 512 x 512`. To achive this, using the `ConvTranspose2d` layer from PyTorch, which is the opposite of a convolution called as a **transposed convolution** or **deconvolution**.

![image](https://user-images.githubusercontent.com/79587733/149307300-e0de0a35-077b-43d3-9b93-0b9d13404735.png)

## Results

<img src="https://user-images.githubusercontent.com/79587733/149310980-58aa8ef7-37db-4a96-a115-a6391cac6598.png" style="width:300px; margin-bottom:32px"/>

These are some of the images that have been generated by the model after training for **500 Epochs**.
