# Face Mask Detection

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#purpose-of-project">Purpose of Project</a></li>
    <li><a href="#architecture">Architecture</a></li>
    <li><a href="#technologies">Technologies</a></li>
    <li><a href="#how-to-run">How to run</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

## Purpose of Project

* Train a model to detect if the person is wearing mask or not
* Using Transfer Learning

## Architecture

* This project uses OpenCV to detect the face, then crop it out then use pre-trained model
* Pre-trained model: This model applied Transfer Learning on pre-trained MobileNet. I only trained on last 2 added layers

## Technologies

* Language: Python
* Framework: Tensorflow

## How to run

### Prerequisites

Required Libraries:
* tensorflow
* opencv
* numpy

### Data preparation

* Download the dataset from [here](https://drive.google.com/drive/folders/1-QhgkHW4wdsd37A8iEIfO7RYQY390WUN?usp=sharing)
* Dataset original source: [this paper](https://arxiv.org/abs/2008.08016)

### Train model

Run `Face_Mask_Detection.ipynb`

### Save `my_model.h5`

If you train your model on Google Colab then make sure to download `my_model.h5` to your local machine

### Test model
```
python visualize.py
```
Please do note:
* This model can not detect face with glasses
* This model need to detect your face to run properly
* This model can only detect some kind of mask, not all of them

## Acknowledgments

* Youtube Tutorial: [video](https://www.youtube.com/watch?v=FPRFYYMlhyw)
* Dataset Paper: [paper](https://arxiv.org/abs/2008.08016)
