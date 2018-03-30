## Data Generator for 2D Object Detection
---
### Contents

1. [Overview](#overview)
2. [Dependencies](#dependencies)
3. [How to use it](#how-to-use-it)

### Overview

This is a data generator for 2D object detection with axis-aligned rectangular bounding boxes. Its main focus is on flexible and easily extensible data augmentation.

Main features:
* It lets you easily define arbitrary chains of random or deterministic image transformations.
* It provides most common photometric and geometric image transformations out of the box.
* It let's you
* It provides both random and deterministic versions of all image transformations.
* It provides parsers for ground truth annotations in the MS COCO (JSON) and Pascal VOC (XML) formats as well as a wide range of CSV formats.

Most data generators for training deep neural networks on computer vision tasks that ship with deep learning libraries are limited to image classification and those that I was able to find for 2D object detection are either only applicable to a specific model, provide only a small set of hard-coded and inflexible data augmentation features, are otherwise severely limited, or are just all around terrible pieces of code. When you train a deep neural network on an object detection task, the data augmentation you perform is one of the most important factors that determine the success of your training, therefore I wrote this data generator specifically with the goal of flexible and easily extensible data augmentation.

### Dependencies

* Python 3.x
* Numpy
* OpenCV
* Beautiful Soup 4.x (to parse XML files)

Python 2 compatibility: This implementation seems to work with Python 2.7, but I don't provide any support for it. It's 2018 and nobody should be using Python 2 anymore.

### How to use it

Everything you need to know in order to use this data generator is explained in the following Jupyter notebook:

* [Data Generator Tutorial](data_generator_tutorial.ipynb)
