# Real Time cabbage detection with Tensorflow SSD
This project contains all the different files and scrips used to deploy a realtime
cabbage detection algorithm using Tensorflow object detection API. As work task, 
i was in charge to develop and deploy a realtime object detection for a drone.
Basically, the first step and the most time consuming part was to gather the dataset.
In order to do that, we manually took picture of different cabbage field with different point of view.
If ypu wish to detect a more common object, you can refer to the opensource images database to check if your object is included. Here is the [link](https://storage.googleapis.com/openimages/web/index.html)
From those pictures, we could manually label them by using LabelImg. It produces the xml in PASCALVOC format which is easier to use for the following part. To have more information about how to retrain the tensorflow object detection API, please refer to [this link](https://github.com/tensorflow/models/tree/master/research/object_detection).

The goal of this repository is to show how deep learning can be applied in daily life and also to provide that can be adapted to some other uses case.

## Table of contents

1. [Installation](#instllation)
2. [Utilisation](#utilisation)
3. [Contributing](#contributing)
4. [License](#licence)

## Installation
This model was trained using a NVIDIA GPU. First of all, please install all the NVIDIA requirements as explained in the official website. [Nvidia official page](https://developer.nvidia.com/).  
Secondly please refer to the official [Tensorflow](https://www.tensorflow.org/install/install_linux#tensorflow_gpu_support) website to know the requirements for the tensorflow-gpu.
>Note: I have exported my model with tensorflow 1.12.0.  Using another version may cause errors, so please export the model yourself with the model checkpoint to fit your tensorflow version. The export can be done by following the [step](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/exporting_models.md)here.  

Moreover, I strongly recommend to use virtual environment to do this project else some errors might occur due to the libraries dependencies.  
Virtual environment is good for python development because it can let you having many different working environments which depends on differents libraries without having conflicts.  
If you do not know many about virtual env, [please refer to this excellent tutorial](https://realpython.com/python-virtual-environments-a-primer/)

Please refer to the requirements.txt to install all the others dependencies. Be sure to be in the virtual environment before typing the following command.
- `pip install -r requirements.txt`

## Utilisation

## Contributing

## Licence
Apache Licence. See [LICENSE](LICENSE) for details. Copyright (c) 2018 Enroute.
