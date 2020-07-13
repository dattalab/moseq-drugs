# Revealing the structure of pharmacobehavioral space with Motion Sequencing

This repository contains code to download the raw and processed data from Wiltschko et al., 2020, train and analyze linear classifiers on featurizations of pharmacologically-modified mouse behavior, and analyze the relationships of differing and similar drugs using MoSeq featurizations of behavior.

This code is tested with the Anaconda Python distribution on Python 3. It is a minimal reproduction of the data processing and analysis routines in the paper.

To get started, first clone this repository

```shell
git clone https://github.com/dattalab/moseq-drug-classifier
cd moseq-drug-classifier
pip install -e .
```

Now, we can download the data. This will create a new folder `moseq-drug-classifier/data`.
To download the full dataset, including raw behavioral time-series data, run:

```shell
# To download the full dataset, including full behavioral time-series data
sh ./scripts/download_all_data.sh
```

To just download the behavioral featurizations, run:
```shell
# To just download featurizations of behavior
sh ./scripts/download_featurized_data.sh
```

Now, you can run any number of analysis notebooks on the download data. Please navigate to `moseq-drug-classifier/notebooks` for more.
