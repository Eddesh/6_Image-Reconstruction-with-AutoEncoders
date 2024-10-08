# Image-Reconstruction-with-AutoEncoders

## Project Overview
This project implements an Autoencoder to reconstruct images from the Fashion MNIST dataset. The Autoencoder consists of an Encoder that compresses the image data into a latent space and a Decoder that reconstructs the original image from this compressed representation. This project demonstrates the effectiveness of autoencoders in image reconstruction and compares different model architectures and hyperparameters for improved reconstruction accuracy.

### Dataset Description
The Fashion MNIST dataset, used for training and evaluation, consists of grayscale images of various clothing items. Each image is 28x28 pixels in size and represents one of ten categories: T-shirts/tops, trousers, pullovers, dresses, coats, sandals, shirts, sneakers, bags, or ankle boots. For this project, the dataset is divided into training and test sets, with an additional split for validation during model training. This structure allows for thorough evaluation of the autoencoder’s performance in reconstructing the images.

### Step 1: Data Preprocessing and Splitting
The Fashion MNIST Image Reconstruction with Autoencoders.ipynb notebook includes data preprocessing steps, such as normalization and resizing of images, followed by splitting the dataset into training, validation, and test sets.

### Step 2: Model Training
An Autoencoder model is trained with a combination of convolutional and pooling layers in the Encoder and upsampling layers in the Decoder. The notebook includes various configurations:
Model 1: A simpler architecture with basic layers.
Model 2: Enhanced with Batch Normalization and Dropout for improved performance.

### Step 3: Image Reconstruction and Evaluation
After training, the models reconstruct the test images and evaluate the quality using Structural Similarity Index (SSIM). The results are plotted for visual comparison, showing both original and reconstructed images.
The evaluation metrics and SSIM scores are recorded for further analysis.

## Testing
The project includes two Autoencoder models tested for image reconstruction:

Model 1: This simpler model achieved an average SSIM score of 0.8736, with stable training and validation losses after 25-30 epochs.
Model 2: Enhanced with Batch Normalization and Dropout, Model 2 achieved a higher SSIM score of 0.8833 and converged faster with improved stability.
Both models show effective reconstruction capabilities, with Model 2 providing slightly better results in terms of SSIM and visual quality.

## Author
Davin Edbert Santoso Halim
