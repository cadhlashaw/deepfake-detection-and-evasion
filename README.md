# Deepfake Detection and evasion

This repository contains the code used for ELE8095 individual research project,investigating deepfake detection, adversarial attacks and defences.

#Overview

The project compares a baseline XceptionNet detector with a dual-stream CombinedDetector incorporating spatial and frequency-domain features.

#The experiments include:

- DeepFakes and FaceShifter subsets from FaceForensics++
- FGSM and PGD white-box attacks
- Black-box transfer attacks
- Adversarial fine-tuning
- Gaussian low-pass filtering
- Frequency-branch evaluation and refinement
- Cross-dataset testing using StyleGAN-generated faces
- Post-result gated-fusion and frequency-branch diagnostic analysis

#Dataset 

The processed experimental dataset contained:
- 8,000 real frames
- 4,000 DeepFakes frames
- 4,000 FaceShifter frames


The processed FaceForensics++ subset used in this project is not included in the repository due to its size, but can be provided if required.

A separate subset of the 140k Real and Fake Faces dataset was used for the StyleGAN frequency-branch experiments.
https://www.kaggle.com/datasets/xhlulu/140k-real-and-fake-faces.


## Repository Contents

The notebooks contain the implementations and experiments relevent to the final report.

## Environment

Dataset subset creation, frame extraction and file organisation were carried out locally using Visual Studio Code.
Experiments were primarily carried out in Google Colab using PyTorch with CUDA-enabled GPUs.

## Code References

Some implementation details were informed by publicly available documentation, tutorials and open-source examples, including:

-The FGSM and PGD attack implementations were informed by code and examples provided in teaching material from ELE8100.

-PyTorch documentation and timm 
https://pprp.github.io/timm/models/xception/
https://docs.pytorch.org/docs/2.14/generated/torch.fft.fft2.html

Informed by :

https://danielsdiscoveries.wordpress.com/2017/09/29/spectrogram-input-normalisation-for-neural-networks/
https://github.com/huggingface/pytorch-image-models/blob/main/timm/models/xception.py
- GeeksforGeeks website was utilised many times for python help throughout the project 
eg. "Implementation of a CNN based Image Classifier using PyTorch" – used as a general reference


Ideas and motivation for architecture:

https://pdfs.semanticscholar.org/1143/e556afe8a910ab9da86c7ca763838ae37efc.pdf
https://arxiv.org/pdf/2511.19187



AI: 

AI was used in generating graphs and imaging,and was used as assistance in debugging my original code ideas.


