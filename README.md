# GAN-VAE-logo-generation
This repository contains three main notebooks that explore different approaches to logo generation and similarity analysis using the LLD dataset:

- Deep Convolutional GAN (DCGAN)
Implements a Deep Convolutional Generative Adversarial Network (GAN) designed to generate logo variations based on the images in the LLD dataset.

- Variational Autoencoder (VAE)
Implements a Variational Autoencoder (VAE) designed to learn a latent representation of the logos in the dataset and generate new variations using the decoder.

- Feature Extraction & Similarity Analysis (VGG16 + UMAP)
Uses the pre-trained VGG16 network to extract and compare features from the LLD dataset logos and a user-provided logo.

  - A 2D plot with UMAP is generated to visualize the clustering of dataset features.

  - Using Cosine Similarity, the 5 most similar dataset images to the user’s logo are identified.

  - If the user’s logo is too similar to an existing one, a fallback procedure is triggered: our DCGAN and VAE models are used to generate two new logos that still respect the similarity criteria.
