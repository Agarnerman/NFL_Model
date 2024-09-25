# NFL Betting Model
Project Overview:

This repository contains the source code and data for an NFL betting model. The model was developed to predict the outcomes of NFL games based on historical data.

As of 09/22/2024 it has a 68% success rate.

Data Acquisition:

NFL Data: Historical NFL data was scraped from NFL Pro-Reference for the seasons 2014 to 2022. The data was then combined with scraped data from the 2023 season to create a comprehensive dataset.
Vegas Lines: Vegas lines for all the seasons were also scraped and stored in a separate CSV file.
Model Development:

Version 1: The initial version of the model trains a KNeighborsClassifier model to predict Under or Over for NFL games based on historical data of spread and total points.
It also iterates through seasons 2021-2023 and weeks 1-18 to evaluate the model's performance, while analizing the nearest neighbors for test data points.
You would then change the bottom portion of the code for whatever week of games is upcoming, and input the spread and total lines.
Note that the model currently is noticably better at prediciting Unders rather than Overs.

Version 2: The second version incorporated several improvements, including:
LOF: Local Outlier Factor was used to identify and handle outliers in the data.
Pipelines: Pipelines were implemented to streamline the data preprocessing and modeling process.
Scalers: Data scaling techniques were applied to ensure numerical features were on a similar scale.
Masks: Masks were used to selectively include or exclude features during training and evaluation.
Code Structure:

[GatheringData.py],[ExtendingData.py]: Contains functions for scraping NFL data and Vegas lines.
[NFLBettingModel.py]: Implements the first version of the model.
[TweakedNFLModel.py]: Implements the second version of the model with improvements.

Future Work:

Explore additional features and data sources to improve model accuracy.
Experiment with different machine learning algorithms and techniques.
Implement real-time betting strategies based on model predictions.
