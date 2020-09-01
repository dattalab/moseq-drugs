# Revealing the structure of pharmacobehavioral space with Motion Sequencing

This repository contains code from Wiltschko et al., 2020, to train and analyze linear classifiers on featurizations of pharmacologically-modified mouse behavior, and analyze the relationships of differing and similar drugs using MoSeq featurizations of behavior.

This code is tested with the Anaconda Python distribution on Python 3. It is a minimal reproduction of the data processing and analysis routines in the paper.

To get started, first clone this repository

```shell
git clone https://github.com/dattalab/moseq-drug-classifier
cd moseq-drug-classifier
pip install -e .
```

Now, download the data onto your computer. All of the data in the paper is stored on Zenodo at:

```
https://doi.org/10.5281/zenodo.3951698
```

There are three files:

`dataset.pkl` -- this is the full dataset, containing the extracted depth images and scalar info (posiiton, velocity, heading, etc).

`syllablelabels.pkl` -- this is the MoSeq label sequence of each frame of recorded data. This is further processed into a MoSeq fingerprint in the fingerprint file.

`fingerprints.pkl` -- this contains the featurizations of mouse behavior, and associated experimental information per-mouse (such as what drug a mouse was given, at what dose). Featurizations include scalars, MoSeq, shuffled MoSeq, individual scalar data such as height, length, velocity and distance-to-center.

Place the files all in the same directory, accessible from the machine where you wish to run the analysis notebooks. Edit the notebooks accordingly to point to each file. Now, you can run any number of analysis notebooks on the download data. Please navigate to `moseq-drug-classifier/notebooks` for more.
