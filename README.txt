# Binary Classification using SRGAN
The goal of this project is to generate 128x128 images from 32x32 images using SRGAN and inputting these generated images through a binary classifier. This method will be compared with just having the original images inserted into the binary classifier.

# Creating the Binary Classifier
Download the Kaggle Retinal OCT dataset
Import the required libraries
Create the directory to your datasets
Set training parameters
Create data generators using ImageDataGenerator()
Build the binary model and train it on the Kaggle dataset

# Creating the SRGAN
Use the same Kaggle dataset
Import required libraries
Resize the images to 128x128 and 32x32 and store both in their own directories
Define the generator and discriminator models
Train the generator and discriminator for more than 50 epochs on the 32x32 images to be able to generate higher resolution images.


