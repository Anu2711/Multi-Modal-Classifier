# Multi-Modal-Classifier
This repository contains code to train a multi-modal machine learning model that classifies fashion items into 27 categories by utilizing noisy text descriptions, noisy images, and categorical variables. The model trained obtained an 88% accuracy in classifying the test set.

## Dataset Description
The data consists of e-commerce products. Each product has a unique id and a category. We need to predict the category of each product based on categorical features, a noisy text description and a noisy image.

### Data Fields
* id: a unique id for each product
* category: a string describing the category of each product
* gender: a string describing the target gender for this product
* baseColour: the base colour of this product (note that the base colour may be different than the colour in the image of this product)
* season: a string describing the target season for this product
* usage: a string describing the target usage for this product
* noisyTextDescription: a string of words corresponding to a noisy display name of the product

### Images
For each product, there is a noisy image of the product in the directory "noisy-images". The filename of each image is the product id. The images are 60x80x3 jpeg images in RGB format (i.e., each pixel intensity is an integer in {0,1,2,…,255}).

