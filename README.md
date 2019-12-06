## Earthquake Analysis and Prediction

This part of the project is associated with a machine learning and optimization techniques which were used for the prediction of earthquakes and clusters. Various methods are applied taking the raw fields of the original dataset as well as certain useful features extracted from the original dataset as input to the various machine learning models.It was observed that the results improved when the features extracted from the original dataset were used as input to those machine learning models than when the raw fields of the original data were used for the same purpose.

_Note: Data set can be extracted [here](https://www.kaggle.com/usgs/earthquake-database)_

#### Tableau
Tableau's features helped us to perform tasks like sorting, comparing, grouping and visualizing the data.
Click [here](https://public.tableau.com/profile/maria.serobabina#!/vizhome/Earthquakes_15729298219800/CorrelationAnalysis)

#### Machine Learning
To complete machine learning, time series were forecasted using `ARIMA model` where autoarima models were built in python. Using python earthquakes frequency was identified for past 52 years, and then earthquake forecast was made utilizing Arima model. Also a `DBSCAN algorithm` performed clusters analysis in 150 kilometer epsilon bubbles with a minimum grouping of ten based upon USGS earthquake documentation, providing 99.5% compression of 23,412 points down to 116 clusters.

#### Big Data Analytics
Basis `AWS applications` were utilized to store data for this project. After cleaning data in `Python` it was stored on a AWS `S3 Bucket` on cloud storage which was connected to `Zepplin` where data analysis and a graph was plotted.

Finally, the project was deployed on `Heroku`. 
To see the project click [here](https://quakeland.herokuapp.com/)
