# Multimodal Emotion Recognition using Video-Based Datasets
Thanks for your attention. In this repo, we provide the code for the Bilkent University 2019-2020 Spring CS-484-555 Introduction to Computer Vision course final project. 
### Authors:
Mustafa Çağrı Güngör,
Merve Özen,
Nurefşan Müsevitoğlu

## Download Datasets
Crema-D, eNTERFACE'05 datasets and ResNet3D-50-KMS pretrained weights can be downloaded following links, [Crema-D](https://drive.google.com/drive/folders/15fLaAmJnFEaUpx0pqikQqptg5dAkT0QX?usp=sharing), [eNTERFACE'05](https://drive.google.com/drive/folders/1PG9XDSpjduN5ygghUH078XvVoxiB2n0e?usp=sharing) and [ResNet3D-50-KMS](https://drive.google.com/file/d/1Z1agO6kKkMr-RcQz3DTptOORrqma1dQd/view). The samples in the datasets are in the preprosessed format which can be directly used for training.

## Running the Code
1. Place the datasets, pre-trained weights and IPYNB files to the any Google Drive account.
2. Mount the Google Drive account in the environment of Google Colab. The code script below, connects your Google Drive to Colab. The script are included in the first cell of the all IPYNB files.
```
from google.colab import drive 
drive.mount('/mntDrive')
```
3. Change the datasets and pre-trained weights directory according to where it is placed in the Google Drive. The code script below are included in the second cell of the all IPYNB files. 
```
CREMA_D_PATH = "/mntDrive/My Drive/Data/CREMA-D"
pretrain_path = "/mntDrive/My Drive/Data/r3d50_KMS_200ep.pth"
```
4. Enter Runtime menu, change runtime type as GPU (it is needed) and run all cells.
### Note:
While Google Colab running the cell below, the error "[Errno 5] Input/output error:" can be occurred due to tring to access big amount of data. The error is stem from the Google Drive environment and the solution is that run the cell below again, then run all again. The problem will be solved.
```
files = os.listdir(CREMA_D_PATH)
```
