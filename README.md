# Multimodal Emotion Recognition using Video-Based Datasets
Thanks for your attention. In this repo, we provide the code for the Bilkent University 2019-2020 Spring CS-484-555 Introduction to Computer Vision course final project. The code consist of six IPYNB files which are 3D Conv method, CNN-RNN method and Fusion of these methods for both Crema-D and eNTERFACE'05 datasets.
### Authors:
Mustafa Çağrı Güngör,
Merve Özen,
Nurefşan Müsevitoğlu

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
While Google Colab running the cell below, the error "[Errno 5] Input/output error:" can be occurred due to trying to access big amount of data. The error is stem from the Google Drive environment and the solution is that re-run the cell below, then run all cells again. The problem will be solved.
```
files = os.listdir(CREMA_D_PATH)
```
