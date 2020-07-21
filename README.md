# Image-Caption-Generator-Data-Science-
Model used was [ResNET50](https://iq.opengenus.org/resnet50-architecture/) and was trained over RNNs/LSTMs. 

The model was trained on [Flickr8K](https://forms.illinois.edu/sec/1713398) image data set. 

A custom Data Generator was enforced during training which had the work of maintaining RAM usage. 

The results obtained in any time were processed on NVIDIA 1060 3GB GPU.

## Table of Contents

1. [Requirements](#1-requirements)
2. [Training parameters and results](#2-training-parameters-and-results)
3. [Generated Captions on Test Images](#3-generated-captions-on-test-images)

## 1. Requirements

Recommended System Requirements to train model.

<ul type="square">
	<li>A good CPU and a GPU</li>
	<li>Atleast 16GB of RAM</li>
	<li>Active internet connection so that keras can download model weights</li>
</ul>

Required libraries for Python used while making & testing of this project

<ul type="square">
	<li>Python - 3.6.7</li>
	<li>Numpy  </li>
	<li>Tensorflow(GPU) - 2.1.0</li>
	<li>Keras - 2.3.1</li>
	<li>Matplotlib </li>
</ul>


## 2. Training parameters and results

#### NOTE

| Model & Config | Argmax |
| :--- | :--- |
| **ResNET50** <ul><li>Epochs = 20</li><li>Batch Size = 3</li><li>Optimizer = Adam</li></ul> |<ul>**Crossentropy loss**<br>*(Lower the better)*<li>loss(First epoch): 3.1794</li><br><li>loss(Second epoch): 2.9504</li><br><li>... and so on the result of all are listed in main.ipynb</li><br><li>loss(20th epoch): 2.2446</li>  |

## 3. Generated Captions on Test Images

* After the training of the model, Random 15 images were selected from the test set and their captions were generated.
* The Images as well as their generated captions are saved in main.ipynb file so you can check them out.
