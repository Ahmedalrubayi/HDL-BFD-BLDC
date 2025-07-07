## 📘 HDL-BFD-BLDC HTFICNN model :
MATLAB implementation scripts of HTFICNN: a hierarchical time-frequency CNN for bearing fault detection in BLDC motors using scalogram, spectrogram, and Hilbert spectrum features.
Journal of Electrical and Computer Engineering*, 2024  
> [https://doi.org/10.1155/2024/3376733](https://onlinelibrary.wiley.com/doi/full/10.1155/2024/3376733)

## 🧠 Method Overview :
- Abstract: This paper presents a novel Hierarchical Time-Frequency Image-based Convolutional Neural Network (HTFICNN) for sorted bearing fault detection in Brushless DC (BLDC) motors. The HTFICNN integrates a scalogram, a spectrogram, and a Hilbert spectrum to transform current and vibration signals into time-frequency images (TFIs). These are processed by three parallel convolutional paths, each trained to detect faults based on one TFI type. A hierarchical fusion classification combines outputs from all three networks for final decision-making.
Experimental results demonstrate the superiority of HTFICNN over conventional deep models, contributing significantly to intelligent fault diagnosis and predictive maintenance in BLDC motors.
-The proposed method:
- Uses **Continuous Wavelet Transform (CWT)** and **Hilbert-Huang Transform (HHT)** to create scalograms and spectrograms.
- Trains multiple CNN variants for hierarchical fault classification.
- Validates performance on real BLDC motor fault datasets with multiple trained models.

- ## 📦 Contents
- `scripts/`: MATLAB functions for model training, testing
- `models/`: Pretrained networks benchmark models.

## ⚙️ Requirements
- MATLAB R2021a or later
- Deep Learning Toolbox
- Signal Processing Toolbox
- Image Processing Toolbox

## 🗂️ Dataset Preparation
The code requires two image folders:
- dataset_cnn_train/` – contains training scalogram/spectrogram/Hilbert images
- dataset_cnn_test/` – contains test images
-  Each folder should be structured by class, e.g.:
### ⚠️ Note:
Due to size, the dataset is not included in this repository.  
You may:
- Generate the images using your script with native MATLAB functions for signal processing and image processing to create the time-frequency transformation image, including the scalogram, spectrogram, and Hilbert transform.
- Or request the dataset by emailing the author.
- 
## 🚀 Getting Started main scripts:
- HMCNN_training.m
- HMCNNnetwork.m
- Test_Net.m
- training_recent_models.m
- comparison.m
  
📬 Contact
Author: Ahmed Ali
📧 engineer28ahmed@gmail.com

🔖 Citation:
- Ali, A. K., & Rafa Abed, W. (2024). Hierarchical Deep Learning for Bearing Fault Detection in BLDC Motors Using Time‐Frequency Analysis. Journal of Electrical and Computer Engineering, 2024(1), 3376733.‏
