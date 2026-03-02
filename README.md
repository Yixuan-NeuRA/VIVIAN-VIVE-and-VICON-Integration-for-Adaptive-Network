**Description:**  
This is a project for improving the low-cost motion tracking sensor performance close to a gold-standard motion capture system.

Vicon: The Vicon motion capture system is the gold-standard motion capture system in the world (Vicon Motion Systems Ltd., Oxford, UK).  

VIVE: VIVE Ultimate Tracker is a low-cost motion tracking sensor that combines an inertial measurement unit with a simultaneous localisation and mapping algorithm (HTC, Taiwan, China).  

**Data preprocessing:**  
Spatial Position Mapping and Synchronisation of Two Motion Capture Systems with Different Performance Characteristics
DOI: https://doi.org/10.13140/RG.2.2.25764.13440  

**Dataset:**  
VIVIAN_Dataset_V1\vive_vicon_comparison_data.csv  
This dataset is used for the standard task of improving the performance of low-cost motion-tracking sensors toward a gold-standard motion capture system.

VIVIAN_Dataset_V1\vive_vicon_CoM_data.csv  
This dataset is used to map the sacrum tracker's position to the participant's centre of mass (CoM).  

Try to finish these two tasks in the same or a similar machine learning architecture.  

**Code:**  
VIVIAN_V4.1.ipynb  
CNN+Transformer  
VIVIAN_V4.2 (CNN-only).ipynb  
CNN only  
VIVIAN_V4.3 (Transformer-only).ipynb  
Transformer only
