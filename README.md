# Dandelion Cell Analysis

This repository contains several files related to my research project: **Advancing single-cell B cell receptor trajectory analysis with absorbing Markov chains.**

- `read-data-fetal.ipynb` - this notebook was 
- `data-preprocessing.ipynb` - this notebook was used to preprocess the fetal scRNA-seq dataset 
- `drafts` - notebooks created to test and trial different methods to analyse and explore the datasets. Its not necessary or as important or organized as the notebooks above.  

Some of the datasets were too large for Github. instead, these have been uploaded to a separate Google Drive or elsewhere.

Orginal datasets for adult and fetal scRNA-seq can be found here: https://drive.google.com/drive/folders/1dXRPjq7SRMo9x2pCWGbf14Cv4sBcJSCZ?usp=sharing


Additionally, the modified Markov chain required modifying Palantir directly as fork - the repository can be found here: https://github.com/christopheragnus/Palantir

## How to reimplement the analysis

1. Clone this repository
2. Download the BCR metadata from (download all the `dandelion-remap` files too and untar): https://github.com/zktuong/dandelion-demo-files/blob/master/dandelion_manuscript/data/dandelion-remap/BCR_metadata.csv
 

3. Run `data-preprocessing.ipynb` first to process the downloaded dataset. Skip to the BCR Preprocessing section. The output will be written into the `write` folder.
4. Read in the prior output in `read-data-fetal.ipynb` and run the analysis
5. To use the modified markov chain, clone the forked Palantir repository
6. Run and install Palantir in Python's dev mode
7. Run `python data-analysis.py` to execute the analysis