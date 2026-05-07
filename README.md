# ***Description:***  
This is a project to improve the agreement with Vicon, particularly for gait parameters and dynamic stability outcomes, and a sacrum‑only setup can enable accurate CoM position estimates to obtain dynamic stability outcomes.  

***Task 1:*** A data-driven model was trained to correct the raw VIVE Ultimate Tracker (VUT) coordinates to better align with the Vicon marker coordinates at the corresponding tracker locations (sacrum, left foot, and right foot). Gait spatiotemporal and dynamic stability parameters were subsequently computed from three trajectory sources (Vicon, VUT, and model) to evaluate whether coordinate correction improves downstream biomechanical outcomes.  

***Task 2:*** The same model architecture was applied to train and estimate the whole-body CoM derived from full-body Vicon markers using only the sacrum-mounted VUT trajectory as input, and the resulting CoM estimates were used to compute XCoM and MoS and compared with those obtained from raw VUT and the Vicon gold standard. Whole-body CoM from Vicon was computed using a standard segmental approach based on the full-body marker set and anthropometric parameters, yielding a 3D CoM trajectory at 100 Hz for the gold standard in Task 2.  

***Task 1*** constitutes the primary validation of VUT-derived gait outcomes against Vicon, whereas ***Task 2*** is a secondary analysis designed to test whether CoM-derived stability metrics can be enabled under a minimal sacrum-only configuration. 

***Vicon:*** The Vicon motion capture system is the gold-standard motion capture system in the world (Vicon Motion Systems Ltd., Oxford, UK).  

***VUT/VIVE:*** VIVE Ultimate Tracker is a low-cost motion tracking sensor that combines an inertial measurement unit with a simultaneous localisation and mapping algorithm (HTC, Taiwan, China).  

# ***Data preprocessing:***  
Spatial Position Mapping and Synchronisation of Two Motion Capture Systems with Different Performance Characteristics
DOI: https://doi.org/10.13140/RG.2.2.25764.13440

# ***Dataset:***
The dataset for Task 1:
https://github.com/Yixuan-NeuRA/Validation-of-VIVE-and-VICON.

Tha dataset for Task 2:



# ***Code:***  
VIVIAN_V4.1.0.ipynb: CNN+Transformer  
VIVIAN_CoM_V4.1.ipynb: CNN+Transformer
VIVIAN_V4.1.ipynb and VIVIAN_CoM_V4.1.ipynb use the same model architecture and training strategies. 
The trained model will be saved in the current directory by default.


# *Library version:*    
numpy: 1.26.0  
pandas: 2.0.3  
torch: 2.7.0+cu126  
matplotlib: 3.10.3  
sklearn: 1.3.2  
tqdm: 4.67.1  
