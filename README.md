 

# MFG-CRT: Multi-Feature Guided Cross-Refinement Transformer for RGB-Guided Thermal Image Super-Resolution

## Overview of MFG-CRT
MFG-CRT: Multi-Feature Guided Cross-Refinement Transformer for RGB-Guided Thermal Image Super-Resolution

## PREREQUISITES
Prerequisites for MFG-CRT.

## OS
AIR Research Framework is supported on Ubuntu 16.04 LTS or above.

## Python
It is recommended that use Python 3.7 or greater, which can be installed either through the Anaconda package manager or the Python website.

## Pytorch
Recommended that use Pytorch 1.5.0 or above version.
Important: EDVR or some models that have dependency on Deformable Convolution Networks feature only works in Pytorch 1.5.0a0+8f84ded.

## Pull container image
At the first, pull docker container image.
docker pull nvcr.io/nvidia/pytorch:20.03-py3

## Clone
```
git clone https://github.com/DoGunKIM93/MFG-CRT.git
```

## Install some required packages
```
pip install fast_slic munch IQA_pytorch pillow fast_pytorch_kmeans
```

## Dataset
×16 Guided Thermal Image Super-Resolution Dataset
```
datasetPath: 'dataset directory path' (in Param.yaml)
```

## Pre-trained
MFG-CRT Pre-trained
```
pretrainedPath: 'Pre-trained directory path' (in Param.yaml)
```

## Train 
At MFG-CRT folder, type following command:
```
python main.py
```
## Test
At MFG-CRT folder, type following command:
```
python main.py -it
```

## Acknowledgements
This code is built on [AFA-Net](https://github.com/DoGunKIM93/AFA-Net-And-Joint-IRLPRNet), [CRAFT-SR](https://github.com/AVC2-UESTC/CRAFT-SR/tree/main?tab=readme-ov-file).
