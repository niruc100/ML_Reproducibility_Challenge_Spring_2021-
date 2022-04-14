# Introduction

This repository contains the scripts and code of the experiments we conducted for the Machine Learning Reproducibility Challenge 
Spring 2021. The experiments are named after the respective captions from the results
section. The algorithm is implemented in ```train_abs.py``` and ```test_abs.py```, the script to obtain the datasets is ```dataset.py```. The file 
```util.py``` is required to properly plot the results.

# References
This repository contains parts of the original implementation to reproduce the reported results. 

- The original paper: https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123750426.pdf
- The original implementation: https://github.com/CSIPlab/learnPR_reference

# Run The Code
Please follow the instructions below before you run the notebooks.

## Environment
We run our experiments on an jupyter lab server with the following packages:
- numpy 1.21.0
- scikit-image 0.18.1
- pytorch 1.5.0
- torchvision 0.6.0+cu101

You can install the most important packages using:
```pip install -r requirements.txt```

## Download The Data
You need to download and unzip CelebA manually before running some of the notebooks.
For this you can download CelebA from the official source

[CelebA Google Drive Repository](https://drive.google.com/drive/folders/0B7EVK8r0v71pTUZsaXdaSnZBZzg?resourcekey=0-rJlzl934LzC-Xp28GeIBzQ)

and unzip the dataset into a folder named ```./data/```, such that the ```.png ```
images are accessible via ```./data/img_align_celeba```. This is required to load CelebA with the provided script.

## Learn The References
It is required to first run the notebook 
```reconstructions-using-learned-references.ipynb``` as this creates the 
self-trained references that are used in the other notebooks.

## Experiments
At this point, you are ready to run all notebooks in any order. 
