# RealTime-Food-Detection-in-Refrigerator

This repo let's you train a custom food object detector using the  YOLOv3 computer vision algorithm.

## Pipeline Overview

To build and test your YOLO object detection algorithm follow the below steps:
 
 1. [Download Images](/1_Download_Images/)
	 - "Download All Images" is a chrome extension
	 - Downloads all images from a web page and packs them into a zip file.
 2. [Image Annotation](/2_Image_Annotation/)
	 - Install LabelImg
	 - Annotate images
 3. [Training](/3_Training/)
 	- Download pre-trained weights
 	- Train your custom YOLO model on annotated images 
 4. [Inference](/4_Inference/)
 	- Detect objects real time using web-cam
 
## Getting Started

### Google Colab Tutorial <a href="https://colab.research.google.com/github/AntonMu/TrainYourOwnYOLO/blob/master/TrainYourOwnYOLO.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
With Google Colab you can skip most of the set up steps and start training your own model right away. 

### Requisites
The only hard requirement is a running version of python 3.6 or 3.7. To install python 3.7 go to 
- [python.org/downloads](https://www.python.org/downloads/release/python-376/) 

and follow the installation instructions. Note that this repo has only been tested with python 3.6 and python 3.7 thus it is recommened to use either `python3.6` or `python3.7`.

To speed up training, it is recommended to use a **GPU with CUDA** support. For example on [AWS](/2_Training/AWS/) you can use a `p2.xlarge` instance (Tesla K80 GPU with 12GB memory). Inference is very fast even on a CPU with approximately ~2 images per second. If you want to use your own machine, follow the instructions at [tensorflow.org/install/gpu](https://www.tensorflow.org/install/gpu) to install CUDA drivers. Make sure to install the [correct version of CUDA and cuDNN](https://www.tensorflow.org/install/source#linux). 


  
