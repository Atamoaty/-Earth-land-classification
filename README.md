# Land Classification using EuroSAT-RGB

## Project Overview
This project focuses on classifying different land cover types (such as urban, vegetation, water, and barren areas) using the EuroSAT-RGB dataset based on Sentinel-2 satellite imagery.  
It aims to build a deep learning model capable of distinguishing land types from RGB images.

## Dataset
- Name: EuroSAT-RGB (subset of the EuroSAT dataset)
- Source: Sentinel-2 satellite images
- Classes: Agricultural, Forest, Urban, Water, Desert, etc.
- Images per class: approximately 2,000–3,000 (depending on the category)

## Exploratory Data Analysis (EDA)
- Inspected image dimensions and color channels.
- Visualized sample images for each land cover type.
- Identified class imbalance between categories.
- Noted that NDVI and other spectral indices cannot be computed due to missing NIR band (available only in the multispectral version).

## Model Plan (Upcoming Milestones)
1. Preprocess and normalize the images.  
2. Split data into train, validation, and test sets.  
3. Train a CNN model for classification.  
4. Evaluate and visualize performance metrics.

## NDVI and Spectral Notes
The RGB dataset lacks the NIR band, so NDVI cannot be computed.  
If available, NDVI is defined as:

NDVI = (NIR - RED) / (NIR + RED)

High NDVI values indicate dense vegetation,  
while low NDVI values correspond to urban or barren regions.

## Repository Structure
Land_Classification_Project/
│
├── dataset/                
├── Land_Classification_Project.ipynb  
├── README.md               
└── reports/ (optional)

## Author
Omnia Boghdady  
Data Science & Machine Learning Engineer

