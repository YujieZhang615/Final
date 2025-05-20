# Final
🧊 AI4EO: Sea Ice Classification and Roughness Prediction Using Remote Sensing and Machine Learning

📍 University College London – GEOL0069 Artificial Intelligence for Earth Observation

📌 Overview

This project applies artificial intelligence techniques to study sea ice surface roughness and classification using:

Sentinel-1 C-band SAR data (VV, HH, HV)

DEM-derived surface roughness (RMS)

Machine learning models including SVM, KMeans, CNN, and regression

The project aims to support safe sea ice navigation, climate monitoring, and environmental forecasting.

🛰️ Data Sources

Sentinel-1 SAR: VV/HH/HV polarizations (from Google Earth Engine)

DEM: Simulated or photogrammetry-derived digital elevation models (representing ice topography)

Study Areas: Simulated Arctic sea ice near coastlines (e.g., China Arctic coastline / Pond Inlet)

🧠 AI Techniques

Task	Method

Water vs Ice Detection	Threshold on VV backscatter
Ice Type Clustering	KMeans (unsupervised, HH + HV)
Ice Type Classification	SVM, CNN
Roughness Prediction	Linear, Polynomial, Random Forest, GPR
DEM Sensitivity	Gradient-based CNN sensitivity

🧪 Models & Implementation

sea_ice_analysis.ipynb contains all code blocks:

Data loading and visualization

VV thresholding

KMeans clustering (HH, HV)

SVM classification (VV, HH, HV, RMS)

CNN-based classification and roughness mapping

Regression comparison (Linear, Polynomial, RF, GPR)

CNN sensitivity analysis across DEM grids

📈 Sample Outputs

Predicted sea ice types using SVM with VV/HH/HV/RMS features.


Roughness (RMS) map predicted using polynomial regression.

🧪 Reproducibility

pip install -r requirements.txt
Models can be run fully on CPU in Jupyter or Google Colab.

🌍 Environmental Cost

Item	Value
Hardware	CPU (Google Colab)
Training Time	< 1 min per model
Energy Consumption	~0.002 kWh
CO₂ Emissions	~0.001 kg CO₂eq

This project has a low environmental impact, with all training performed on small datasets and light models.


📚 References
Segal et al. (2020). Sea Ice Roughness and SAR

Filipponi (2019). Sentinel-1 Polarimetric Backscatter

ESA Sentinel-1 documentation

GEOL0069 UCL AI4EO module notes


[![Open In Colab]
https://colab.research.google.com/drive/1OMXPyxuHVpiL_-01YQz8FoV015lhdjKp#scrollTo=L9n8ccIcJLjj

