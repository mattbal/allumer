# Allumer
A WSU Crimson Code Hackathon project TIER 1.

Allumer is a mobile app that uses Machine Learning to diagnose your skin patch. Simply take a photo using the app, and Allumer will determine whether or not your skin patch is likely cancerous.


## Tools

### Mockups

Mockups were created using Adobe XD and Google Material Design icons. 

### Machine Learning

Machine learning was created using Keras and Python.

We used this library to train the images: https://www.kaggle.com/fanconic/skin-cancer-malignant-vs-benign#1007.jpg
The library contains ~2,500 images for training that are confirmed skin cancer, as well as 660 testing images.

I built a image classification neural network utilizing keras and tensorflow. Approximatly 2000 photos of malignant and benign skin blemishes/moles were stored in two appropriately named folders within a "train" folder. There were 660 other unique images sorted in a similar fasion within the "test" folder. Numerous layers of filters and other data manipulation functions made up the neural network. After the network was compiled images were resized to fit a standard resolution and transformed into a data type the network could understand.

### iOS Mobile App

The iOS app was created using Xcode and Swift.

