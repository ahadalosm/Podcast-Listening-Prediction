ML Project - Podcast Listening Time Prediction using XGBoost
---

This project was created as part of an exploration into applying machine learning to real-world user behavior. It focuses on predicting how long users will listen to podcast episodes based on episode characteristics, content sentiment, and popularity metrics.

The model uses XGBoost Regressor to estimate listening time with high accuracy and interpretability.

" Project Structure "
---
PodcastPrediction.ipynb:  
- Loads and explores the dataset  
- Preprocesses data (label encoding, scaling)  
- Trains the XGBoost regression model using K-Fold Cross Validation  
- Evaluates performance using RMSE  
- Visualizes feature importance, residuals, and predictions  

train.csv / test.csv:  
The dataset files containing podcast metadata, engagement features, and listening time (target in train.csv only).

submission.csv:  
Final prediction file generated using the trained model on the test set.

" Dataset "
---
Name: Podcast Listening Dataset  
Target: `Listening_Time_minutes`  
Key Features:
- Episode_Length_minutes  
- Number_of_Ads  
- Host_Popularity_percentage  
- Guest_Popularity_percentage  
- Genre  
- Publication_Day / Publication_Time  
- Episode_Sentiment  

This dataset simulates podcast platforms' user engagement metrics for modeling and analysis purposes.


" Tools & Libraries Used "
---
- Python  
- Jupyter Notebook  
- XGBoost  
- Scikit-learn  
- Pandas  
- NumPy  
- Matplotlib & Seaborn


" Project Workflow "
---
1. Load the training and test datasets  
2. Preprocess features (categorical encoding)  
3. Split data using K-Fold Cross Validation  
4. Train an XGBoost Regressor model  
5. Evaluate model using RMSE  
6. Analyze feature importance and residuals  
7. Predict test data and generate submission


" Results "
---
- Cross-validated RMSE: 12.891 ± 0.008
- Most important feature: Episode_Length_minutes
- Final predictions distributed between 0 to 120 minutes

The model showed consistent performance across all folds and successfully captured key patterns in user listening behavior.


" Author "
---
Ahad Alosaimi  
Data & AI Developer – 2025
