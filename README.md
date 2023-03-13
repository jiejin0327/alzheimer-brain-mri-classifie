# alzheimer-brain-mri-classifier

This project aims to classify brain MRI images of Alzheimer’s disease into four categories: NonDemented, VeryMildDemented, MildDemented and ModerateDemented. It uses ResNet50 as a base model with a custom classifier layer on top.

## Installation
To use this project, you need to have Python 3 and Jupyter Notebook installed on your machine. You can also run it on Google Colab if you prefer.

You also need to download the dataset from [Kaggle](https://www.kaggle.com/datasets/sachinkumar413/alzheimer-mri-dataset) and place it in the same folder as the notebook file.

Additionally, you need to download the pre-trained weights for ResNet50 from [here](https://drive.google.com/file/d/12kgtrjPKAUGo-TXf43aTRHna4eU1rJwf/view?usp=sharing) and save them as *resnet50_weights.h5* in the same folder.


## Usage
To run this project, simply open the notebook file alzheimer-brain-mri-classifier.ipynb and follow the instructions there. You can also modify the code as you wish to experiment with different settings or models.


## Model Introduction
This project uses ResNet50 as a base model, which is a deep convolutional neural network that can handle complex image recognition tasks. ResNet50 has a special feature called residual blocks, which allow each layer to learn from its previous layers and avoid degradation problems. This improves the accuracy and generalization ability of the model.

On top of ResNet50, this project adds a fully connected layer with 256 units and a dropout rate of 0.5, followed by a softmax layer with 4 units for classification. The model is trained using Adam optimizer with a learning rate of 0.0001 and categorical crossentropy loss function.

## Parameter Settings
This project uses the following parameters for image preprocessing and model training:

* Image size: 224 x 224
* Image color mode: RGB
* Batch size: 16
* Learning rate: 0.0001
* Training epochs: 50

## Results
This project achieves an accuracy of 97% on test dataset and performs well on all classes
