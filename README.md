# Fundamentals of Data Analysis Project
### Hayley Doherty

The aim of the project in this notebook is to perform and explain simple linear regression on a dataset which is able to accuratelt predict an output for a given input value.

The notebook begins with an explanation of linear regression and what it can be used for.  I then begin analysis of the dataset which contains data regarding the wind turbine power output for a range of wind speed values.  

First the NumPy polyfit function is used to determine the coefficients of the line of best fit, which weere then used to graph the line over the dataset.  These coefficients could then be used to predict output values for given values of x.
Next the linear model function from the Scikit learn package was used to perform linear regression on the dataset.  The model was trained and again used to predict power output from a wind speed value.  The predicted value given by the Scikit learn package was much higher compared to the predicted value calculated from the NumPy polyfit coefficients.

Following this analysis I removed what I deemed to be outlying data points from the dataset to determine what affect this might have on modelling the data and getting accurate predictions.  The same methods for modelling, training the dataset as well as making predictions were used as above.  This time the values returned for the prediction of power output were identical for the two methods.  The score calculated for the Scikit learn model which calculated the accuracy of the model was also much higher with this dataset compared to the previous sata which still contained the outlying data points (0.6789 vs. 0.9033).