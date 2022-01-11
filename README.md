# Predicting incidence of heart disease

SWBio DTP Data Science and Machine Learning 

## Background 
Heart failure is a highly prevalent and progressive condition, clinically defined as a cardiac abnormality causing cardiac output to be insufficient to meet the body’s
metabolic requirements [1]. Heart failure currently affects an estimated 26 million people worldwide with prevalence set to increase [2]. 
With early detection of heart disease considered vital for successful clinical intervention, there is much interest in the use of machine learning to aid in medical diagnosis [3].

## Motivation 
Using the publicly available Heart Failure Prediction dataset [4], containing various clinical variables of people with and without heart disease, I aim to design a 
supervised machine learning model which can be used to accurately predict heart disease. This project is a binary classification, with the aim to predict incidence 
of heart disease based on multiple clinical variables. Annotated code has been written using a Jupyter notebook (version 3.2.1.) using Python 3.9.7. 

I have first pre-processed the data, checking for missing or null values, and checking the distribution of the variables in the dataset.
I have then generated a correlation matrix comparing correlation coefficients between heart disease and the numerical variables in the dataset, using seaborn [7],
and carried out some exploratory data analysis of the different variables in the dataset. I then generated various supervised learning binary classification models 
imported from SciKit Learn [5] and compared using model scores and ROC curves to see which best predicts heart disease.

To run:
1.	Download Heart Failure Prediction dataset “heart.csv” (originally downloaded from Kaggle: https://www.kaggle.com/fedesoriano/heart-failure-prediction). 
2.	Open jupyter notebook "DataScienceAssessment" and check file path to ensure "heart.csv" file is read in correctly. 
3.	Run entire notebook, generating following outputs: import of pandas, NumPy, matplotlib, seaborn and SciKit learn libraries [5-10], correlation matrix, scatter matrix, graphical analyses of relationship between target variable heart disease and explanatory variables, generation of 5 binary classification models (Logistic Regression, Naïve Bayes, KNearest Neighbors, SVC and Decision Trees), generation of confusion matrix comparing model scores and ROC curves comparing each model. 


In my analysis, I have found the best performing classification model for prediction of the target variable HeartDisease to be the Support Vector Machines (SVC) model, 
with a model score of 0.86 (2.d.p.) and an ROC AUC score of 0.92. 

However, future work would be required to further optimise the hyperparameters for each model to ensure optimal model performance. 

## Acknowledgements:
I would like to thank both Matt Williams and Chris Woods for their incredibly helpful tutorials. 

## References:
[1] Remme, W.J. & Swedberg, K. (2001) Task Force for the Diagnosis and Treatment of Chronic Heart Failure, European Society of Cardiology, Guidelines for the diagnosis and treatment of chronic heart failure, European Heart Journal, Volume 22, Issue 17, Pages 1527-1560, https://doi.org/10.1053/euhj.2001.2783

[2] Savarese, G., & Lund, L. H. (2017). Global Public Health Burden of Heart Failure. Cardiac failure review, 3(1), 7–11. https://doi.org/10.15420/cfr.2016:25:2

[3] Yasmin, F. et al. (2021) Artificial intelligence in the diagnosis and detection of heart failure: the past, present, and future. Rev. Cardiovasc. Med., 22(4), 1095–1113. https://doi.org/10.31083/j.rcm2204121 

[4] fedesoriano. (September 2021). Heart Failure Prediction Dataset. Retrieved [17th December 2021] from https://www.kaggle.com/fedesoriano/heart-failure-prediction.

[5] Pedregosa, F. et al. (2011). Scikit-learn: Machine learning in Python. Journal of machine learning research, 12(Oct), pp.2825–2830.

[6] Van Rossum, G. & Drake, F.L. (2009). Python 3 Reference Manual, Scotts Valley, CA: CreateSpace.

[7] Waskom, M. L., (2021). seaborn: statistical data visualization. Journal of Open Source Software, 6(60), 3021, https://doi.org/10.21105/joss.03021

[8] Hunter, J. D. (2007). "Matplotlib: A 2D Graphics Environment", Computing in Science & Engineering, vol. 9, no. 3, pp. 90-95.

[9] Harris, C.R. et al. (2020). Array programming with NumPy. Nature, 585, pp.357–362.

[10] Reback, J. et al. (2020). pandas-dev/pandas: Pandas 1.0.3 (v1.0.3). Zenodo. https://doi.org/10.5281/zenodo.3715232



