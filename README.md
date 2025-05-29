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



A figure illustrating the remote sensing technique and/or a figure illustrating the AI algorithm and its implementation

![ChatGPT Image 2025年5月21日 15_07_37](https://github.com/user-attachments/assets/0f3ebaee-c4c6-4af1-8bdf-6a2c2359335b)
![ChatGPT Image 2025年5月21日 15_09_09](https://github.com/user-attachments/assets/054e04c1-80bf-4723-8cb9-f86bead822c9)



🌍 Environmental Cost

Item	Value
Hardware	CPU (Google Colab)
Training Time	< 1 min per model
Energy Consumption	~0.002 kWh
CO₂ Emissions	~0.001 kg CO₂eq

The environmental impact of this research project is minimal, as it relies primarily on digital data processing and analysis using existing datasets (e.g., satellite imagery and DEMs). No physical fieldwork, sample collection, or use of chemical materials is involved, thereby eliminating direct environmental disturbances.

The main environmental cost stems from the computational energy consumption associated with model training, data simulation, and evaluation. This includes:

Running machine learning models (e.g., CNNs, Random Forests)

Using cloud computing resources (e.g., Google Colab, local GPUs)

Storage and transfer of large geospatial datasets

To minimize this footprint, the project employs the following sustainability practices:

Efficient code execution and model optimization to reduce runtime and energy use

Use of lightweight models (e.g., shallow CNNs, downsampled inputs) wherever possible

Training with a limited number of epochs and small batch sizes

Leveraging cloud platforms with carbon-neutral commitments (e.g., Google Cloud)

Overall, the project is designed to be low-impact, with its computational requirements carefully managed to reduce unnecessary emissions. Moreover, the research itself contributes positively to environmental monitoring (e.g., sea ice classification, roughness estimation), supporting sustainable decision-making in polar and climate-sensitive regions.


📚 References
Segal et al. (2020). Sea Ice Roughness and SAR

Filipponi (2019). Sentinel-1 Polarimetric Backscatter

ESA Sentinel-1 documentation

GEOL0069 UCL AI4EO module notes


Python code：
https://colab.research.google.com/drive/1OMXPyxuHVpiL_-01YQz8FoV015lhdjKp#scrollTo=L9n8ccIcJLjj

Vedio link: https://youtu.be/gbKllYvHn7I

