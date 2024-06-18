# Denoising-image

Background and Objective
Image denoising is a crucial preprocessing step in various computer vision applications, aimed at enhancing the quality of images by removing noise. This project focuses on developing a convolutional neural network (CNN) model from scratch for image denoising, avoiding the use of pre-trained models. The primary goal is to train the model on a dataset of noisy and clean images, evaluate its performance using metrics such as Mean Squared Error (MSE), Peak Signal-to-Noise Ratio (PSNR), and produce denoised images for a test set.

Architecture Used
The architecture used in this project is a simple yet effective CNN designed specifically for denoising tasks. The model consists of several convolutional layers followed by max-pooling and up-sampling layers to capture both the local and global features of the image. The key specifications of the architecture are:
Input Layer: Takes a grayscale image of size 128x128.
Convolutional Layers: Three convolutional layers with 64, 32, and 32 filters, respectively, all using a 3x3 kernel size and ReLU activation.
Max-Pooling Layers: Two max-pooling layers to down-sample the feature maps, reducing the spatial dimensions by half.
Up-Sampling Layers: Two up-sampling layers to restore the original image dimensions.
Output Layer: A convolutional layer with a single filter and sigmoid activation to produce the final denoised image.

Implemented Paper
This project is inspired by various research papers in the field of image denoising. One notable paper is "Image Denoising by Sparse 3D Transform-Domain Collaborative Filtering" by K. Dabov, A. Foi, V. Katkovnik, and K. Egiazarian. The paper presents an advanced denoising algorithm based on collaborative filtering in a 3D transform domain, known as BM3D. While our model does not directly implement BM3D, it leverages similar principles of capturing spatial correlations in images. The paper can be accessed : "https://ieeexplore.ieee.org/document/4299272"
