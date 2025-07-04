# Gender Classification Project 🎯

This project uses Transfer Learning with a pre-trained ResNet18 model to classify images into Male or Female based on facial features.

# Model Weight

Model weight (.pth file) are stored on google drive due to file size limits.

## Download Model Weights here

https://drive.google.com/file/d/1vhJKAPdhcAvIwZ1xyte5J_17PdqFVqx6/view?usp=sharing

## Model Architecture,Validation loop and training loop

https://github.com/Anushkasaha1/Gender-Classification-Project/blob/main/gender-classification-project.py

## 🧠 Model Architecture
The gender classification model uses ResNet18 as its backbone. The architecture is modified as follows:

Backbone:

ResNet18 pre-trained on ImageNet

Custom Classification Head:

Original fully connected layer (fc) replaced with:

Linear layer (512 → 512 units)

ReLU activation

Dropout (e.g. probability 0.3) to reduce overfitting

Linear layer (512 → 2 units) for binary classification (male / female)

This design enables the network to learn high-level facial features while adapting specifically to gender prediction.


 # 🚀 Project Overview--
  1.Model: ResNet18 (pre-trained on ImageNet) 

  2.Framework: PyTorch 3.Task: Gender Classification from facial images 
# 🔧 Tools & Libraries--
 1.Python 

 2.PyTorch

 3.TorchVision 

 4.Google Colab 

# 📊 Achievements-- 
1.Validation Accuracy: ~91% 

2.Successfully able to predict gender from unseen images. 

# ⚠ Limitations-- 
 1.Model trained only on frontal face images.
 
 2.May misclassify images with extreme lighting, blur, occlusion, or multiple faces..
