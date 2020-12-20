# Covid-19 Trend Report

By Tobias Kächele (https://tobiaskaechele.de)

This Jupyter Notebook analyzes the dataset of newly confirmed cases from John Hopkins and outputs an up-to-date trend report for a small selection of countries. It is based on a Monte-Carlo simulation to generate multiple interpolations of a trend curve - using the Savitzky-Golay filter to smoothen the data - and determines the likelihood of a positive or negative trend of each day. Finally, a report in the form of a single HTML file is generated listing the countries and the current trend.

You can find a complete explanation of the math behind it on my blog:<br>
https://tobiaskaechele.de/blog/Trend-Analysis-of-New-COVID-19-Cases


## Requirements

* Python 3.7+
* Jupyter Notebook *or* Jupyter Lab
* Python packages Matplotlib, pandas, SciPy, NumPy, and tqdm (see below on how to install them).


## How to Use

1. Clone git repository or just download the Jupyter Notebook

2. Install the packages Matplotlib, pandas, SciPy, NumPy, and tqdm:<br>
   ```pip install matplotlib, pandas, scipy, numpy, tqdm```

3. Run all cells in the Jupyter Notebook. The newest data from John Hopkins will be downloaded automatically.

4. The generated trend report can be found in the output directory:<br>
   `./output/report.htm`