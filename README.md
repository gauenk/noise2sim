# Noise2Sim -- Similarity-based Self-Learning for Image Denoising
By [Chuang Niu](https://scholar.google.com/citations?user=aoud5NgAAAAJ&hl) and [Ge Wang](https://www.linkedin.com/in/ge-wang-axis/)

## Introduction
This project is the Pytorch implementation of the [paper](https://arxiv.org/abs/2011.03384).

## Installation
Assuming [Anaconda](https://www.anaconda.com/) with python 3.6, the required packages for this project can be installed as:
```shell script
conda install pytorch==1.4.0 torchvision==0.5.0 cudatoolkit=10.1 -c pytorch
conda install faiss-gpu cudatoolkit=10.0 -c pytorch
conda install matplotlib
conda install -c conda-forge python-lmdb tqdm imageio addict tensorboard opencv
```
Then, clone this repo
```shell script
git clone https://github.com/niuchuangnn/noise2sim.git
cd noise2sim
```

## Run
To train the model, simply run the following commands.

Run for BSD68,
```shell script
python ./tools/train_dist.py --config-file ./configs/stl10/bsd400_unet2_ps3_ns8_gpu1.py
```

## Citation

```shell
@inproceedings{noise2sim2021,
  title={Noise2Sim – Similarity-based Self-Learning for Image Denoising},
  author={Niu, Chuang and Wang, Ge},
  booktitle={arXiv:2011.03384},
  year={2020}
}
```