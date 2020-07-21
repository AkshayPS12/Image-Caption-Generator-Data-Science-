# Image-Caption-Generator-Data-Science-
Model used was [ResNET50](https://iq.opengenus.org/resnet50-architecture/) and was trained over RNNs/LSTMs. 

The model was trained on [Flickr8K](https://forms.illinois.edu/sec/1713398) image data set. 

A custom Data Generator was enforced during training which had the work of maintaining RAM usage. 

The results obtained in any time were processed on NVIDIA 1060 3GB GPU.

## Table of Contents

1. [Requirements](#1-requirements)
2. [Training parameters and results](#2-training-parameters-and-results)
3. [Generated Captions on Test Images](#3-generated-captions-on-test-images)
4. [Procedure to Train Model](#4-procedure-to-train-model)
5. [Procedure to Test on new images](#5-procedure-to-test-on-new-images)
6. [Configurations](#6-configurations-configpy)
7. [Frequently encountered problems](#7-frequently-encountered-problems)
8. [TODO](#8-todo)
9. [References](#9-references)

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
	<li>nltk  </li>
	<li>PIL </li>
	<li>Matplotlib </li>
	<li>tqdm </li>
</ul>


## 2. Training parameters and results

#### NOTE

| Model & Config | Argmax |
| :--- | :--- |
| **ResNET50** <ul><li>Epochs = 20</li><li>Batch Size = 3</li><li>Optimizer = Adam</li></ul> |<ul>**Crossentropy loss**<br>*(Lower the better)*<li>loss(train_loss): 2.4050</li><li>val_loss: 3.0527</li>**BLEU Scores on Validation data**<br>*(Higher the better)*<li>BLEU-1: 0.596818</li><li>BLEU-2: 0.356009</li><li>BLEU-3: 0.252489</li><li>BLEU-4: 0.129536</li></ul> |<ul>**k = 3**<br><br>**BLEU Scores on Validation data**<br>*(Higher the better)*<li>BLEU-1: 0.606086</li><li>BLEU-2: 0.359171</li><li>BLEU-3: 0.249124</li><li>BLEU-4: 0.126599</li></ul> |

