# Bayesian Image Super-Resolution

## Overview
Bayesian super-resolution is a technique used to enhance the resolution of images by incorporating Bayesian inference principles. It involves estimating the likelihood function for the image registration parameters through marginalization over the unknown high-resolution image, as proposed by Tipping and Bishop. This approach allows for the estimation of the unknown point spread function and is made tractable by introducing a Gaussian process prior over images.

This repository contains the implementation of a Bayesian super-resolution algorithm using PyTorch proposed by Tipping et al. ([link to paper](https://proceedings.neurips.cc/paper_files/paper/2002/file/88bfcf02e7f554f9e9ea350b699bc6a7-Paper.pdf)).

## Features
- Generates high-resolution (HR) images from low-resolution (LR) inputs.
- Utilizes Bayesian inference to incorporate prior knowledge and uncertainty estimation.
- Supports various image transformation and optimization techniques.
- Includes utilities for image preprocessing, evaluation, and visualization.

## Usage
1. Clone the repository.
2. Install dependencies.
3. Set the correct path of the high-resolution image.
4. Run the notebook.

## Example
Here is an example  :

| High Resolution Image | Low Resolution Image | Patch | Bilinear Interpolation | Reconstructed High Resolution |
|-----------------------|----------------------|-------|-------------------------|-------------------------------|
| ![High Resolution Image](Results\monaliza.png) | ![Low Resolution Image](Results\LR_monaliza.png) | ![Patch](Results\Patch_LR.png) | ![Bilinear Interpolation](Results\monamliza_binr.png) | ![Reconstructed High Resolution](Results\monaliza_GP.png) |

## Reference
- Michael Tipping and Christopher Bishop. Bayesian image super-resolution. Advances in neural information processing systems, 15, 2002. [Link to Paper](https://proceedings.neurips.cc/paper_files/paper/2002/file/88bfcf02e7f554f9e9ea350b699bc6a7-Paper.pdf).
