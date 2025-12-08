# Implementing Variational Autoencoders

### This github repository showcases the code I created on my journey to understanding variational autoencoders (VAEs). In vae.ipynb you will find the code I used to create and train a multilayer linear VAE from scratch, with no machine learning libraries. vae.ipynb also contains the code I used to create a multilayer convolutional variational autoencoder (CVAE), which was built and trained using PyTorch. The linear VAE was trained on the MNIST handwritten digit dataset to generate images of handwritten digits from 0-9. The CVAE was trained on a lower-resolution version of the the Labeled Faces in the Wild (LFW) dataset, a dataset containing >13,000 images of >5,000 celebrities. 

![lfw_gif](https://github.com/user-attachments/assets/f43df30a-62bf-4f81-b2fb-7b39760d7f51)

### How to Run the Models to Generate Images:

This GitHub repository contains files that have pretrained weights for both the linear VAE and the convolutional VAE, so no model training is required to generate images with the models. Follow the steps below to use the models to (only) generate images:

1. Clone the github repository to your machine.
2. Create a virtual environment and download all the requirements in the requirements.txt file.
3. Open vae.ipynb and **run every cell individually (except cells where train() is called)**. Do not use "run all" because if you are not training a model, some variables will be undefined and the kernel will stop executing cells.
4. Go to the bottom of the notebook to the cell that says "Run this code if you only just want to use the pretrained models to generate new images".
5. Alter the `model_path` variable to be your desired model from the `models/` directory.
6. Run the cell :).
