Denoising Diffusion Probabilistic Models Implementation in Pytorch
========

This repository implements [DDPM](https://arxiv.org/abs/2006.11239) with training and sampling methods of DDPM and unet architecture mimicking the stable diffusion unet used in diffusers library from huggingface from scratch.
## Sample Output by trained DDPM on Mnist

<img src="https://github.com/explainingai-code/DDPM-Pytorch/assets/144267687/a8095bc2-a525-40ad-a0ae-ec53da4145b5" width="300">


## Data preparation
For setting up the mnist dataset:
1. Download the MNist dataset and name it as mnist_train.csv
2. 
Follow - https://github.com/explainingai-code/Pytorch-VAE#data-preparation


## Configuration
* ```config/default.yaml``` - Allows you to play with different components of ddpm  


## Output 
Outputs will be saved according to the configuration present in yaml files.

For every run a folder of ```task_name``` key in config will be created

During training of DDPM the following output will be saved 
* Latest Model checkpoint in ```task_name``` directory

During sampling the following output will be saved
* Sampled image grid for all timesteps in ```task_name/samples/*.png``` 

## Citations
```
@misc{ho2020denoising,
      title={Denoising Diffusion Probabilistic Models}, 
      author={Jonathan Ho and Ajay Jain and Pieter Abbeel},
      year={2020},
      eprint={2006.11239},
      archivePrefix={arXiv},
      primaryClass={cs.LG}
}
```
