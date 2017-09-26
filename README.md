# predicting-dengue
Alex Freeman - 9/19/17

DrivenData is currently hosting a competition to predict cases of Dengue Fever in San Juan, Puerto Rico and Iquitos, Peru. The competition can be found here: https://www.drivendata.org/competitions/44/dengai-predicting-disease-spread/

This repository includes: The dataset as provided by the competition website in the datasets folder, my personal submissions so far in the submissions folder. I have rewritten multiple of the models, so it is not possible to reproduce some of these submissions, a data dictionary - dengue data dictionary.txt, iPython Notebooks going through the data science pipeline.
The notebooks follow logically along the numbered order. The unnumbered notebooks are extra modelling techniques:

* `1 - Dengue cases data cleaning.ipynb` - Cleaning, fill in missing values, etc.

* `2 - Dengue cases EDA.ipynb` - Explore the feature set of weather variables

* `3 - Dengue cases EDA.ipynb` - Create a cleaned pandas DataFrame file to load from in later notebooks

* `4 - Predict based on months only.ipynb` - Find and plot the monthly trend

* `5 - Predict residuals with rolling weather data.ipynb` - Use the monthly trend to find residuals and see which weather features to use.

* `6 - DENGUE - BEST MODEL.ipynb` - The solution code for my best performing model.

Extra notebooks:

* `DENGUE - predict on log(cases).ipynb` Take the log of the cases and repeat modelling process

* `Dengue ARIMA.ipynb` - Try the ARIMA method

* `Predict outbreaks & low case classes.ipynb` - Try classification models using models to predict if it is an 'outbreak' or a 'lull' in cases

* `Residuals from seasonality Model.ipynb` - Remove the monthly trend from the cases and use weather features to predict residuals.

* `Dengue Time Series Models.ipynb` - Try multiple different time-based models

* `Predict based on months and rolling or shifted data.ipynb` - Create new features from rolling mean, rolling standard deviation and shifted weather data to predict the residuals.

* `XGBoost predictions.ipynb` - Try the XGBoost model to predict the residuals.
