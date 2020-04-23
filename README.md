# Masked Face Image Recognition Model

This repository contains a TensorFlow based image classification model using a Convolutional Neural Network.
The model can be used to detect if a face in a given image is wearing a mask.

The model is using the `RFMD_part_1` [public dataset](https://github.com/X-zhangyang/Real-World-Masked-Face-Dataset) as the training and testing data sets,
And is based on the [white paper](https://arxiv.org/pdf/2003.09093.pdf) released by Wuhan University researchers.

## Prerequisites

* Python 3
* TensorFlow
* Jupyter Notebook

You will need to `pip3 install` the required modules in the `notebook/masked-detection-tf.ipynb` Jupyter notebook.

## Setup for training

Download the Real world masked face recognition dataset from [here](https://github.com/X-zhangyang/Real-World-Masked-Face-Dataset#download-datasets).
Extract the data and create two directories, `train` and `validation` with the following structure:

```
with_mask
no_mask
```

I recommend to take ~30% of the individual directories inside the `train` directory and move them to the validation directory.
The notebook assumes this data structure resides in a `D:` drive. You can change the path in the notebook code.
