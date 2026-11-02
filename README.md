# EPA Air Quality: Sampling

Sampling analysis of EPA carbon monoxide air quality data in Python, done as part of a Coursera data course. The notebook draws random samples of AQI values and uses the central limit theorem to show how sample means behave.

## Notebook

* `epa_sampling.ipynb`: random sampling with replacement, point estimates, the sampling distribution of the mean, and standard error

## What it covers

* Sampling with `sample()`, with and without a fixed `random_state`
* Comparing a sample mean to the population mean
* Simulating 10,000 samples of 50 AQI values and computing the mean of each
* Plotting the sampling distribution against a normal curve
* Calculating the standard error of the mean

## Key findings

* The population mean AQI is about 6.76, calculated from 260 values with none missing
* A single sample of 50 gave a mean of about 5.54, so one sample can miss the population mean
* Across 10,000 samples, the mean of the sample means was about 6.76, almost identical to the population mean
* The sampling distribution is roughly bell shaped even though the underlying AQI values are right skewed, as the central limit theorem predicts
* The standard error of the mean for the first sample of 50 was about 0.74
* A row index can appear twice in a sample because sampling with replacement returns each drawn row to the pool

## Tools

Python, pandas, numpy, matplotlib, scipy, statsmodels, Jupyter Notebook

## Data

 `c4_epa_air_quality.csv`
