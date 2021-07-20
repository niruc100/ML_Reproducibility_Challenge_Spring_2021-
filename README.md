# Introduction

This repository contains the scripts and code of the experiments we conduct for our ML Reproducibility Challenge 
Spring 2021. The experiments are named after the captions of the results
section. The algorithm is implemented in ````train_abs.py``` and ```test_abs.py````
, the script to obtain the datasets is ```dataset.py``` and 
```util.py``` is required to plot the results.

# Run the code

## Environment
We run our experiments in:
- numpy 1.21.0
- scikit-image 0.18.1
- pytorch 1.5.0
- torchvision 0.6.0+cu101

You can install the most important packages with:
```pip install -U requirements.txt```

## Download the data
You need to download and unzip CelebA manually before running the notebooks.
For this you can download CelebA from the official source:


[CelebA Google Drive Repository](https://drive.google.com/drive/folders/0B7EVK8r0v71pTUZsaXdaSnZBZzg?resourcekey=0-rJlzl934LzC-Xp28GeIBzQ)

and unzip the dataset into a folder named ```./data/```, such that the .png 
images are accessible via ```./data/img_align_celeba```.

## Learn the references
It is required to first run the notebook 
```reconstructions-using-learned-references``` as this provides the 
self-trained references that are used in the other notebooks.
