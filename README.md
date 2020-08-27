# Skin Cancer Detection

### Dermatologist-AI

The goal of this mini-project is to build a deep learning model that help to diagnose melanoma,the deadliest form of skin cancer. It will distinguish this malignant skin tumor from two types of benign lesions(Nevus,seborrheic keratoses).

The model trained and tested on several pretrained networks on google colab.

![](https://github.com/parth1620/Skin-Cancer-Detection/blob/master/images/skincancer.png)

### Data

The data and objective are pulled from the [2017 ISIC Challenge on Skin Lesion Analysis Towards Melanoma Detection](https://challenge.kitware.com/#challenge/583f126bcad3a51cc66c8d9a). As part of the challenge, participants were tasked to design an algorithm to diagnose skin lesion images as one of three different skin diseases (melanoma, nevus, or seborrheic keratosis). In this project, you will create a model to generate your own predictions.

* Download and unzip the [training data](https://s3-us-west-1.amazonaws.com/udacity-dlnfd/datasets/skin-cancer/train.zip) (5.3 GB).

* Download and unzip the [validation data](https://s3-us-west-1.amazonaws.com/udacity-dlnfd/datasets/skin-cancer/valid.zip) (824.5 MB).

* Download and unzip the [test data](https://s3-us-west-1.amazonaws.com/udacity-dlnfd/datasets/skin-cancer/test.zip) (5.1 GB).

### Loss and Accuracy

| Pre-trained Networks | Training Loss | Val Loss | Test Loss |
| -------------------- | :-----------: | :------: | :-------: |
| VGG-19bn             |    0.28235    | 0.69861  |  0.72403  |
| ResNet-152           |    0.51237    | 0.67908  |  0.73769  |
| DenseNet-161         |    0.45070    | 0.67656  |  0.70075  |
| Inception-v3         |    0.65855    | 0.92983  |  0.81117  |

 

| Pre-trained Networks | Training Acc | Val Acc | Test Acc |
| -------------------- | :----------: | :-----: | :------: |
| VGG-19bn             |    91.30%    | 72.63%  |  70.72%  |
| ResNet-152           |    78.07%    | 70.59%  |  63.69%  |
| DenseNet-161         |    82.61%    | 68.56%  |  68.12%  |
| Inception-v3         |    70.21%    | 57.71%  |  65.41%  |

 ### ROC AUC Evaluation



**CATEGORY 1 : ROC AUC for Melanoma Classification **

**CATEGORY 2 : ROC AUC Melanocytic Classification **

**CATEGORY 3 : Mean ROC AUC**



* ### VGG-19bn

  ![](https://github.com/parth1620/Skin-Cancer-Detection/blob/master/images/ROC_VGG-19bn.png)

CATEGORY 1 Result : **0.75**

CATEGORY 2 Result : **0.87**

CATEGORY 3 Result : **0.81**



Confusion Matrix with **Threshold 0.25**

![](https://github.com/parth1620/Skin-Cancer-Detection/blob/master/images/CM_VGG19bn.png)

* ### ResNet-152

  ![](https://github.com/parth1620/Skin-Cancer-Detection/blob/master/images/ROC_ResNet152.png)

CATEGORY 1 Result : **0.76**

CATEGORY 2 Result : **0.85**

CATEGORY 3 Result : **0.805**



Confusion Matrix with **Threshold 0.25**

![](https://github.com/parth1620/Skin-Cancer-Detection/blob/master/images/CM_ResNet152.png)

* ### DenseNet-161

  ![](https://github.com/parth1620/Skin-Cancer-Detection/blob/master/images/ROC_DenseNet161.png)

CATEGORY 1 Result : **0.78**

CATEGORY 2 Result : **0.85**

CATEGORY 3 Result : **0.815**



Confusion Matrix with **Threshold 0.25**



![](https://github.com/parth1620/Skin-Cancer-Detection/blob/master/images/CM_DenseNet161.png)

* ### Inception-v3

  ![](https://github.com/parth1620/Skin-Cancer-Detection/blob/master/images/ROC_Inceptionv3.png)

CATEGORY 1 Result : **0.69**

CATEGORY 2 Result : **0.79**

CATEGORY 3 Result : **0.74**



Confusion Matrix with **Threshold 0.25**



![](https://github.com/parth1620/Skin-Cancer-Detection/blob/master/images/CM_Inceptionv3.png) 
