***Description:***  
This is a project for improving the low-cost motion tracking sensor performance close to a gold-standard motion capture system.

Vicon: The Vicon motion capture system is the gold-standard motion capture system in the world (Vicon Motion Systems Ltd., Oxford, UK).  

VIVE: VIVE Ultimate Tracker is a low-cost motion tracking sensor that combines an inertial measurement unit with a simultaneous localisation and mapping algorithm (HTC, Taiwan, China).  

***Data preprocessing:***  
Spatial Position Mapping and Synchronisation of Two Motion Capture Systems with Different Performance Characteristics
DOI: https://doi.org/10.13140/RG.2.2.25764.13440  

***Dataset:***  
VIVIAN_Dataset_V1\vive_vicon_comparison_data.csv: This dataset is used for the standard task of improving the performance of low-cost motion-tracking sensors toward a gold-standard motion capture system.

VIVIAN_Dataset_V1\vive_vicon_CoM_data.csv: This dataset is used to map the sacrum tracker's position to the participant's centre of mass (CoM).  

Try to finish these two tasks in the same or a similar machine learning structure.  

*Variables in the datasets:*  
Subject: Individual IDs of 10 participants (HW3-001 to HW3-010)  
Speed: Four participant walking speeds (0.5, 1.0, 1.5, 2.0 m/s), which do not affect performance and can be ignored.  
Point: Sensor positions in three body locations (1: sacrum, 2: right foot, 3: left foot)  
Direction: 3D coordinate system X, Y, Z  
ViconRowlndex: Timing frame count of the motion capture system (1-5000)  
VIVERowlndex: Timing frame count of the sensor (1-5000)  
Vicon: Data from the motion capture system  
VIVE: Data from the sensor  

***Code:***  
VIVIAN_V4.1.ipynb: CNN+Transformer  
VIVIAN_V4.2 (CNN-only).ipynb: CNN only  
VIVIAN_V4.3 (Transformer-only).ipynb: Transformer only  
These three codes are completely identical except for their model structures.  
Library version:    
numpy: 1.26.0  
pandas: 2.0.3  
torch: 2.7.0+cu126  
matplotlib: 3.10.3  
sklearn: 1.3.2  
tqdm: 4.67.1  
