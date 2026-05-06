#Description:  
This is a project for improving the low-cost motion tracking sensor performance close to a gold-standard motion capture system.
Task 1:
Task 2:

Vicon: The Vicon motion capture system is the gold-standard motion capture system in the world (Vicon Motion Systems Ltd., Oxford, UK).  

VUT/VIVE: VIVE Ultimate Tracker (VUT) is a low-cost motion tracking sensor that combines an inertial measurement unit with a simultaneous localisation and mapping algorithm (HTC, Taiwan, China).  

***Data preprocessing:***  
Spatial Position Mapping and Synchronisation of Two Motion Capture Systems with Different Performance Characteristics
DOI: https://doi.org/10.13140/RG.2.2.25764.13440

***Dataset:***
The dataset for Task 1:
https://github.com/Yixuan-NeuRA/Validation-of-VIVE-and-VICON.

Tha dataset for Task 2:



***Code:***  
VIVIAN_V4.1.0.ipynb: CNN+Transformer  
VIVIAN_CoM_V4.1.ipynb: CNN+Transformer
VIVIAN_V4.1.ipynb and VIVIAN_CoM_V4.1.ipynb use the same model architecture and training strategies. 
The trained model will be saved in the current directory by default.


*Library version:*    
numpy: 1.26.0  
pandas: 2.0.3  
torch: 2.7.0+cu126  
matplotlib: 3.10.3  
sklearn: 1.3.2  
tqdm: 4.67.1  
