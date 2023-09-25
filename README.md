# GAN-image-detection
This repository contains a GAN-generated image detector developed to distinguish real images from synthetic ones.
The complete description of the methodology is available [here](https://arxiv.org/pdf/2203.02246.pdf).
The detector is based on an ensemble of CNNs.
The backbone of each CNN is the EfficientNet-B4.
Each model of the ensemble has been trained in a different way following the suggestions presented in [this paper](https://ieeexplore.ieee.org/abstract/document/9360903) in order to increase the detector robustness to compression and resizing.

## Run the detector

### Prerequisites
1. Create folder for python in IDE or Visual Studio keep thr command module with python to experiment the output value


2. verify the model's weights 


### Test the detector on a single image
We provide a simple script to obtain the model score for a single image.
```bash
python gan_vs_real_detector.py --img_path $PATH_TO_TEST_IMAGE
```

## Performance
We provide python  with the script for computing the ROC curve for each dataset.

