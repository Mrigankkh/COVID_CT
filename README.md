# COVID_CT

In this project I have classfied CT-scans to detect COVID-19 using CNN Networks. Since the dataset was very small , I made use of a pretrained DenseNet model.

# Contents
1. Python Libraries
2. Understanding the dataset
3. Key- points
4. Model Architecture 
5. Training the model
6. Prediction

#  Python Libraries
TorchXrayvision

Torch

Torchvision

Matplotlib

Numpy

Sklearn

# Understanding the Dataset
The dataset contains 425 images of CT-scans of patients as the train data and 203 image s of CT-scans as the test data. The dataset is small and it challenged me to find better ways to implement pretrained models. More information can be found about the dataset at https://arxiv.org/pdf/2003.13865.pdf.

# Key-points 
In this project , the test accuracy alone does not capure the true performance of the model. We need additional parameters such as precision , F1 and area under the ROC curve(AUC). For all parameters, the higher the better. 

# Model Architecture
A pre-trained DenseNet model was used from the torchxrayvision library which is a library for chest X-ray datasets and models. Including pre-trainined models. These models along can be found at https://github.com/mlmed/torchxrayvision



# Training the model
I trained this model in an online cloud instance on Google Colab over 50 epochs.

  # Performance

The model achieved 74.44% accuracy.

Precision: 0.686046511627907

F1: 70.24%

AUC: 81.12%
