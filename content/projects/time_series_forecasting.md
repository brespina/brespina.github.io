+++
title = "time series forecasting on housing prices" 
description = "python, pandas, numpy, scikit-learn, opencv. using publicly available data from zillow and the federal government, i created predictions on what the price would be in the next quarter."
weight = 1

[extra]
local_image = "/projects/time-series-image.png"
+++


painpoints of being my first model. not knowing the difference between tabular vs time-series data. for a long time i was cross validating the model just as i would for tabular data, with k-fold sliding window. however, the temporal nature and order of the data is imperative and must be maintained for all train test splits. so i used expanding window k-fold.

__updated__: 10/17/2024

__todo__: finish explanation, provide metric images

[github](https://github.com/brespina/AIPS/tree/main/Final_Project)
