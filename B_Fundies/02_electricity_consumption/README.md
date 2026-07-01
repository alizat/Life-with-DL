# Electricity Consumption

## Files
- `electricity.ipynb` : jupyter notebook with the code
- `LD2011_2014.txt` : dataset, obtained from [here](https://archive.ics.uci.edu/dataset/321/electricityloaddiagrams20112014)

The following dataset info is taken directly from the website above where the dataset was accessed:
```
- Data set has no missing values.
- Values are in kW of each 15 min. To convert values in kWh values must be divided by 4.
- Each column represent one client. Some clients were created after 2011. In these cases consumption were considered zero.
- All time labels report to Portuguese hour. However all days present 96 measures (24*4). Every year in March time change day (which has only 23 hours) the values between 1:00 am and 2:00 am are zero for all points. Every year in October time change day (which has 25 hours) the values between 1:00 am and 2:00 am aggregate the consumption of two hours.
```

That is to say, for each 15 min interval, the electricity consumption for this interval has been recorded, resulting in 96 (24*4) records per day. Apparently, there are slightly shorter/longer days in March/October, respectively.

From the name of the data file, it appears that these data are for 4 years from 2011 to 2014.

## What is in the notebook?
- Sequential models were trained on the above-mentioned electricity consumption dataset. This is treated as a time-series problem where future consumption levels are to be predicted based on previously seen consumption levels.
- Models considered here are RNN, LSTM and GRU
- Predictions are to be done on 3 levels of granularity
    - per 15-minute interval
    - per day
    - per week
- Comparisons between the considered models in terms of prediction performance
