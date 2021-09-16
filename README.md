# Colorization of Black and White pictures

This repo contains a jupyter notebook which contains the implementation of Autoencoder which transform black and white picture into colorful images using Deep Learning.

The training data were present on the google drive which were accessed from jupyter notebook

Before training we preprocess our data from RGB channels to Lab.

RGB - Red Blue Green
Lab - L refers to Lightness and ab refers to color channels.

#About the model

 * The encoder part consists of convolutional layers with activation ReLu adn strides= 2 for decreasing thw width and height of the latent space vector
 * The decoder part consists of convolutional layers with upscaling layers to restore the dimesions of the original input image (256 x 256) and reconstruct the iamge with 2  filters at the last layer which represents the *ab channels
 * Loss function used in the model while training is L<sub>2<sub>
 * Used Adam as the optimizer 
 
