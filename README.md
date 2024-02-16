# Microscope Slides Fungi Classification using ResNet Models

This repository contains a Google Colaboratory notebook for classifying microscope slides of various fungi using pre-trained ResNet models, including ResNet-18, ResNet-34, and ResNet-101. The notebook is structured with separate sections for model definitions, device diagnostics, training and validation loops, and a test loop.

## Dataset Source
The dataset used in this project was obtained from [HERE](https://www.kaggle.com/datasets/camilovu/lemm-raw). It consists of microscope images of different fungi species, which will be used to train, validate, and test the classification models.

## Models
Three ResNet models are utilized in this project:
- **ResNet-18**: A lightweight version of ResNet with 18 layers.
- **ResNet-34**: A deeper version of ResNet with 34 layers.
- **ResNet-101**: A much deeper version of ResNet with 101 layers.

Each model is defined in a separate section of the notebook, allowing for easy comparison of their performance in classifying the microscope slides.

## Choosing Models
- To use different models you will have to change line 5 under **Device Agnostic Code** to model (ResNet 18), model_34 (ResNet 34), or model_101 (ResNet 101)
- The model chosen will also need to replace lines 18 and 21 under **Train and Validation Loops** to match. 
- Finally, line 4 under **Test Loop** must reflect the changes in the above cells.

## Device Agnostic Code
Before running the classification tasks, the notebook includes code for device agnostic to ensure proper hardware acceleration and compatibility. This section helps in setting up the runtime environment for optimal performance.

## Train and Validation Loops
The notebook contains code for training and validation loops for each ResNet model. These loops are responsible for training the models on the provided dataset and evaluating their performance on a separate validation set. Training metrics such as accuracy, loss, and validation accuracy are monitored during this process.

## Test Loop
Once the models are trained and validated, a separate test loop is included to evaluate their performance on unseen data. This section helps in assessing the generalization capabilities of the trained models.
