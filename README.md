## Earthquake Analysis and Prediction

#### Fetching and plotting earthquakes from the USGS feed.

Java application fetches earthquake data from the USGS website and puts the earthquakes on a map. The background imagery-composite of the map is delivered by using:
* Python
* Flask-powered API
* HTML/CSS
* Java Script
* Leaflet
* D3.js
* MongoDB

The size and color of each marker reflects the magnitude of the earthquake represented. To prevent the map from being overloaded, a minimum threshold for the magnitude, clusters, anamaly of the earthquakes shown can be set as well a map format can be changed.

This project is also associated with `machine learning` and optimization techniques which were used for the `prediction` of earthquakes and `clusters`. Various methods were applied taking the raw fields of the original data set while other useful features were extracted from the original data set as input to the various machine learning models. It was observed that the results improved when the features extracted from the original data set were used as input to those machine learning models than when the raw fields of the original data were used for the same purpose.

The USGS National Earthquake Information Center defines a number of data exchange formats to communicate seismic event processing information between seismic data services and/or algorithms that occur worldwide. These formats are defined using objects as defined in the `JSON standard`. Our data set contains all significant earthquakes with magnitude of 5.5 or higher which have occured from 1965 to 2016.

_Note: Data set can be extracted [here](https://www.kaggle.com/usgs/earthquake-database)_

#### Tableau
Tableau's features helped us to perform tasks like sorting, comparing, grouping and visualizing the data.
Click [here](https://public.tableau.com/profile/maria.serobabina#!/vizhome/Earthquakes_15729298219800/CorrelationAnalysis)

#### Machine Learning
To complete machine learning, time series were forecasted using `ARIMA model` where autoarima models were built. Using python the earthquakes frequency was identified for past 52 years, and then the earthquake forecast was made by utilizing Arima model. Also a `DBSCAN algorithm` performed clusters analysis in 150 kilometer epsilon bubbles with a minimum grouping of ten based upon USGS earthquake documentation, providing 99.5% compression of 23,412 points down to 116 clusters.

#### Big Data Analytics
`AWS applications` were utilized to store data for this project. After cleaning data in `Python` it was stored on a AWS `S3 Bucket` on cloud storage which was connected to `Zepplin` where data analysis was done and a graph was plotted.

Finally, the project was deployed on `Heroku`. 
To see the project click [here](https://quakeland.herokuapp.com/)
