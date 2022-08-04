# Classification of the variable stars from the light curve data from GAIA 3 Data Release
- In this project, we have used the dataset from the GAIA 3 data release 
### Problem Statement
Classifying the periodic variable stars across the 4 categories given below:
1. RR Lyrae
2. Cepheids
3. Long period Variable Stars
4. Eclipsing Binary Stars

- For the extraction of the data we used a library in python called Astroquery. We have downloaded around 50 GB of data. Since, the resources were limited and we selected the data 1 lakh points in each dataset based on classification score. This is also done to eliminate the data imbalance. 

- We started from the 1D convolutional model and tried several other time series models and found that the stacked LSTM model with interpolation and time as input is found to generalize well for the other bands. But for the G band LSTM with only magnitude as input is found to work well. 
