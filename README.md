# alzheimer-brain-mri-classifier
model : ResNet50  
[Download weight data](https://drive.google.com/file/d/12kgtrjPKAUGo-TXf43aTRHna4eU1rJwf/view?usp=sharing)  

**parameter setting**  
  * color mode = rgb  
  * batch size = 16  
  * learning rate = 1e-4  
  * epoch =50 
 
**result**  
  * val_accuracy = 97%  
  
The dataset is downloaded from kaggle [Alzheimer MRI Preprocessed Dataset](https://www.kaggle.com/datasets/sachinkumar413/alzheimer-mri-dataset)


# alzheimer-brain-mri-classifier

This project uses ResNet50 model to perform multi-class classification on brain MRI images of Alzheimer's disease. The dataset comes from [Kaggle](https://www.kaggle.com/tourist55/alzheimers-dataset-4-class-of-images) , which contains four classes: Normal, Non-Alzheimer's Mild Cognitive Impairment (MCI), Alzheimer's Mild Cognitive Impairment (AD-MCI), and Alzheimer's Disease (AD). The dataset has a total of 5121 images, of which 4096 are used for training and 1025 are used for testing.

### alzheimer-brain-mri-classifier

This project uses ResNet50 model to perform multi-class classification on brain MRI images of Alzheimer's disease. The dataset comes from [Kaggle](https://www.kaggle.com/tourist55/alzheimers-dataset-4-class-of-images) , which contains four classes: Normal, Non-Alzheimer's Mild Cognitive Impairment (MCI), Alzheimer's Mild Cognitive Impairment (AD-MCI), and Alzheimer's Disease (AD). The dataset has a total of 5121 images, of which 4096 are used for training and 1025 are used for testing.

## Usage

  * This project uses Jupyter Notebook to show the process of building, training and evaluating the model. You can run Notebook locally or on Google Colab.
  * model : ResNet50  
[Download weight data](https://drive.google.com/file/d/12kgtrjPKAUGo-TXf43aTRHna4eU1rJwf/view?usp=sharing)  


## Model Introduction
This project uses ResNet50 as a base model, and adds a fully connected layer and a Softmax layer on top of it for classification.

Effectively solve degradation problem in deep neural networks i.e., when network layers increase training error increases instead of overfitting.ResNet50 introduces residual block which enables each layer to learn residual function between input & output thus improving accuracy & generalization ability.This project uses pre-trained ResNet50 weights trained on ImageNet dataset & freezes first few layers & trains last few layers only.

## Parameter Settings
This project uses following parameter settings:

* Image size: 224 x 224
* Image color mode: RGB
* Batch size: 16
* Learning rate: 0.0001
* Training epochs: 50

## Results
This project achieves an accuracy of 97% on test dataset & performs well on all classes.
