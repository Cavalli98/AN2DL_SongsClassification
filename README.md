# Politecnico di Milano - Time Series (Songs) Classification challenge for Artificial Neural Network and Deep Learning course


This is the model used in the Time Series Classification Challenge as part of the "Artificial Neural Networks and Deep Learning" course at Politecnico di Milano in 2022.
The goal of the challenge was to classify time series belonging to 12 different classes. Each sample had 6 continuous features.

## Model details

For more details about the model check the [Report](https://github.com/Cavalli98/AN2DL_SongsClassification/blob/main/report/Report.pdf). Briefly, we used the following techniques:
* We tested different models: BLSTM, GRU, Transformers, 1DCNN. The final model is a ResNet with some final layers for classification.
* Data augmentation using the library [tsaug](https://tsaug.readthedocs.io/en/stable/index)
* Test-Time data augmentation (self-ensemble technique) with shifts and flips
* Class weighting to fight the imbalance of the dataset

## Set up
1. Download the dataset from [here](https://drive.google.com/file/d/1uaK_kzFDFelW9z4Voceb5jiX-MdR-4Fa/view) and save the zip inside the data folder.
2. Run the model
