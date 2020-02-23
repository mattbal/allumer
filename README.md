# Allumer. Skin cancer diagnosis reinvented.

Allumer is a Tier 1 WSU Crimson Code project made by Evan Kimmerlein and Matt Balint.

Did you know that skin cancer is the most common type of cancer in the world? In the U.S. alone, approximately 1 million Americans are diagnosed with skin cancer each year. While the survival rate for skin cancer is high, there are still thousands who die each year from not being diagnosed early and there are millions who could benefit from determining whether they have skin cancer or not.

Allumer is an iOS app that uses Machine Learning to diagnose your skin patch. Simply take a photo using the app, and Allumer will determine whether or not your skin patch is likely cancerous.

## Tools

### Mockups

Mockups were created using Adobe XD and Google Material Design icons. 

### Machine Learning

Machine learning was created using Keras and Python.

We used this library to train the images: https://www.kaggle.com/fanconic/skin-cancer-malignant-vs-benign#1007.jpg
The library contains ~2,500 images for training that are confirmed skin cancer, as well as 660 testing images.

Evan Kimmerlein:  I built a image classification neural network utilizing keras and tensorflow. Approximatly 2000 photos of malignant and benign skin blemishes/moles were stored in two appropriately named folders within a "train" folder. There were 660 other unique images sorted in a similar fasion within the "test" folder. Numerous layers of filters and other data manipulation functions made up the neural network. After the network was compiled images were resized to fit a standard resolution and transformed into a data type the network could understand. The network was then trained with batch sizes of 20 and 15 epochs using the images within the "train" folder. Once complete, I used the network to predict the whether the images whithin the "test" folder. By referencing this with the actual values those images should have I got a good estimate of the accuracy of the model - 76%. The was then exported and ready for use on individual images.

### iOS Mobile App

The iOS app was created using Xcode and Swift.

