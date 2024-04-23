# MNIST Deblurring Project
This project involves deblurring images from the MNIST dataset. The blurred version of the images is obtained through a superposition of slightly translated versions of the same image, following a random trajectory. This type of blur is intended to simulate the result of a shot taken with a shaky hand or with a long exposure time.

Images are obtained from the MNIST dataset using a suitable generator provided in the attached notebook.

## MNIST Dataset

The MNIST dataset is a widely-used benchmark dataset in the field of machine learning. It consists of 60,000 training images and 10,000 testing images of handwritten digits (0-9). The dataset is available at: [MNIST Dataset](http://yann.lecun.com/exdb/mnist/)

## Evaluation Metric

The Mean Squared Error (MSE) is used to evaluate the error between the deblurred image and the ground truth. It is computed over 10,000 blurred versions of the test set.

## Experimental Procedure

The computation is repeated 10 times, and the result is the mean MSE over the ten rounds, along with the standard deviation.
