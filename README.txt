#Binary Classification using SRGAN (Super-Resolution Generative Adversarial Network)
This project aims to develop a machine learning model that can generate a higher-resolution image from a 32x32 image which would then be fed into a binary classifier to obtain similar results to a binary classifier being fed the original image with sizes varying around 128x128.

#Installation
To run the code, you’ll need to have the following libraries/modules installed:
* Tensorflow
* Keras
* NumPy
* Matplotlib
* OpenCV
* OS
* PIL

#Dataset
The dataset used in this project was the Kaggle Retinal OCT dataset. However, the dataset used in this project is the tiny version of the original dataset which contains 2000 training images and 500 testing images.

#Preprocessing
Before using the images, the images within the dataset were all scaled to 128x128 images using the Image function from the PIL library and placed into another folder.

#Model
There are three models defined in the project.
* Generator Model
* Discriminative Model
* SRGAN Model

#Running the code
To run the code, a data generator is required. The data generators were created using the ImportDataGenerator module. After that, the SRGAN model is initialized and takes a 32x32 input. Fit() is then performed on the SRGAN to train the model over 100 epochs with callbacks to generate an image and store it into a separate file. 

#Future Plans
The outcome for this project isn’t what was expected. The goal of this project was to insert a 32x32 image and obtain a higher-resolution image.  However, the product of this project was a picture that didn’t seem to look any better than the downscaled version of the original image. In fact, it looked worse. Future plans for this project is to fix the SRGAN model.

#Conclusion
The purpose of this project was to compare the performance of training a binary classifier on the original kaggle dataset with the performance of training a binary classifier on the SRGAN generated images. However, the SRGAN generated images in this project couldn't be made sense of. Therefore, I concluded that it wasn't worth inserting those SRGAN generated images into the binary classifier.
