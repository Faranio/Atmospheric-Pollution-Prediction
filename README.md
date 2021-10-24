# Atmospheric Pollution Prediction

## Requirements

  * Python 3.7+
  * macOS or Linux (Windows not officially supported, but might work)

## Installation (on Ubuntu 18.04):

First, make sure you have anaconda installed. Then you can install gcc with:

```bash
conda install gcc
```

The project utilizes the Prophet library. Therefore it also needs to be installed with:

```bash
conda install -c conda-forge prophet
```

Other necessary packages include jupyterlab, matplotlib, pandas, scikit-learn, seaborn, statsmodels:

```bash
conda install -c conda-forge jupyterlab, matplotlib pandas scikit-learn seaborn statsmodels
```

## Storage

All of the necessary files are stored inside the *data* folder. The structure of the *data* folder is the following:

```
data
│
└───01_raw
│   │   ...
│
└───02_processed
│   │   ...
│   
└───03_graphs
│   │   ...
│   
└───04_results
    │   ...
```

Raw data is stored inside the *data/01_raw* folder. It includes stations data, temperature, and coordinates data.

The *data/02_processed* folder contains cleaned and preprocessed datasets that does not contain missing values for feature columns.

All of the visualizations and graphs of feature data are stored inside the *data/03_graphs* folder.

The last folder *data/04_results* contains resultant prediction CSV files and graphs for each of 10 stations in Moscow city.