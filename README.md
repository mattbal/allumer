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

The iOS app was created using Xcode and Swift. We used Swift UI, a new tool in Xcode/Swift to design the app and tried to implement the mockups designed earlier. As we will explain further below, we ran into quite a few problems trying to build the app, mainly that Swift and iOS have undergone significant updates in the last 2 years, rendering most code over 6 months deprecated.

## Problems we faced


### iOS

As mentioned earlier, the majority of tutorials we tried to follow on YouTube would not compile properly in Xcode because iOS/Swift had been updated significantly since the video was made. Even videos as recent as 6 months ago sometimes did not work due to sheer amount of changes. Additionally, we had problems trying to load the python script/ML model onto iOS. We tried using Firebase and Google's ML Kit, but their ML Kit didn't support Keras and our converted Tensorflow Lite model didn't work properly because it stripped out too much of the Keras functions. Additionally, when we tried to convert our model to Apple's Core ML, it still didn't work because Core ML does not support most Tensorflow functions.

There are also 3 ways to build an iOS app (Storyboards, programmatically or Swift UI). Since you have to stick with which method you choose, a lot of tutorials were difficult to work with because we would often have to modify the code significantly.

