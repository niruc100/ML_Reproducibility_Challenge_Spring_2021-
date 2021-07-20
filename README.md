# Introduction

This repository contains the scripts and code of the experiments we conduct for our ML Reproducibility Challenge 
Spring 2021. The experiments are named after the captions of the results
section. The algorithm is implemented in ```train_abs.py``` and ```test_abs.py```, the script to obtain the datasets is ```dataset.py``` and 
```util.py``` is required to plot the results.

# References
This repository contains parts of the original implementation to reproduce the reported results. 

- The original paper: https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123750426.pdf
- The original implementation: https://github.com/CSIPlab/learnPR_reference

# Run the code
To run our code properly, please follow these steps.

## Environment
We run our experiments on an jupyter lab server with the following packages:
- numpy 1.21.0
- scikit-image 0.18.1
- pytorch 1.5.0
- torchvision 0.6.0+cu101

You can install the most important packages using:
```pip install -U requirements.txt```

## Download the data
You need to download and unzip CelebA manually before running some of the notebooks.
For this you can download CelebA from the official source:

[CelebA Google Drive Repository](https://drive.google.com/drive/folders/0B7EVK8r0v71pTUZsaXdaSnZBZzg?resourcekey=0-rJlzl934LzC-Xp28GeIBzQ)

and unzip the dataset into a folder named ```./data/```, such that the ```.png ```
images are accessible via ```./data/img_align_celeba```. This is required to load CelebA with the provided script.

## Learn the references
It is required to first run the notebook 
```reconstructions-using-learned-references.ipynb``` as this creates the 
self-trained references that are used in the other notebooks.

## Experiments
At this point, you are ready to rerun all notebooks in any order. 
