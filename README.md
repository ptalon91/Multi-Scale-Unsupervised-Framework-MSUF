# Multi-Scale-Unsupervised-Framework-MSUF
This is an implementation of our paper: A Multi-Scale Framework with Unsupervised Learning for Remote Sensing Image Registration.
## Preparation
Our code is performed in Pytorch 1.8.0 basis on Python 3.8.
## Introduction
network.py: Our DNN architectures, implemented on three scales.

generation.py:  Generate the trainging or testing data (image pairs) by datasets provided by the paper or your own datasets.

loss.py: Store various loss functions.

train.py : Training Process.

test.py: Testing Process.

STN.py: Affine Transformation based on STN.

CFOG.cp38-win_amd64.pyd: Similarity evaluation for multi-modal images is recommand as the NCC of the Chanel Feature of Orientated Gradient (CFOG). We provide this executable version of the CFOG descriptor, You could use 'import CFOG' to call this descriptor or adopt thr other descriptors (i.e. HOPC, HOG or LSS) in your code.
## Datasets
The multi-modal original image pairs adopted in the paper have been to Google Drive. You could download them and put them into generation.py to generate the training or testing image pairs.

Optical-Optical dataset: https://drive.google.com/file/d/1U0fpCnizcl33TgdRwvfQpqOr1Ojcj6a9/view?usp=sharing

Optical-Infrared dataset:

Optical-SAR dataset:

Optical-RasterMap dataset:
