# MalariaPredictionFromSatellite2020


## Research Plan
Malaria harms human health and devastates socioeconomic conditions in low-income countries. There were 230 million infections and 420,000 deaths last year. Though there has been enormous progress since the 2000s, progress has plateaued in recent years, and innovative methods are needed to address the challenge. 

Remote sensing temporal variables such as temperature, humidity, rainfall, etc., were used to predict malaria caseload for continents or countries using mathematical models. The accuracy of said models varies significantly for local areas because of the inconsistent local temporal data and parameters that impact malaria transmission. I believe malaria caseloads can be predicted more accurately using a machine learning model that uses the spatiotemporal variable vegetation index in conjunction with temporal variables for small local areas such as towns, districts, or cities. 

I plan to build a machine learning model using remote sensing parameters such as satellite observed vegetation index, local weather, and historical malaria caseload to improve caseload prediction accuracy. I have divided the process into five steps.
Data Download - Download data from Google earth engine/NASA's earth data API, historical malaria caseload data from the public domain/malaria atlas database.
Clean and prepare various datasets- Pre-process the data into a machine-consumable format, calculate vegetation index, etc. Prepare different datasets from training, testing and validation.
Build the model - The Neural net model written using Python and TensorFlow.
Train the model - Training the model using training dataset and model algorithm written in python.
Analyze results - Analyze results and formulate plots and visual maps based on results.


## Abstract
It has been estimated that malaria has been responsible for more deaths than any other disease in human history. Despite progress being made since 2000, the rate of reduction has been stagnant in Sub-Saharan Africa. Researchers have been trying to find innovative approaches for predictions of malaria outbreaks using machine learning. The use of spatiotemporal features has proven useful, but many of said factors are non-deterministic. I focused on applying NDVI in my model, which was examined using sixteen years of training data and three years of validation data from Ibadan, Nigeria.

NDVI (Normalized Difference Vegetation Index) was calculated using MODIS/006/MOD13Q1 satellite image collection dataset with the Google Earth Engine API. NDVI uses the colors of visible and near-infrared sunlight reflected by plants to calculate the vegetation present in a given area. Theoretically, malaria cases should be more prevalent with higher NDVI values. 

I developed six different machine learning models: linear regression, lasso regression, decision tree, random forest, feed-forward neural network, and generalized additive model to predict malaria prevalence. 
I found that NDVI was not as highly correlated to prevalence as I assumed, with total and monthly rainfall being the feature vectors that were most highly correlated. Lasso regression performed the best and led me to find that a limited number of variables can produce a usable model.

My data-driven approach could help local healthcare systems anticipate caseloads with limited spatiotemporal data, which is critical for rapidly emerging urban settlements in Sub-Saharan Africa.
