# An RNN based approach to classify HIV-1 geonmes into HIV-1 subtypes. 

## Problem Definition

The classification of infections among the subtypes of human
immunodeficiency virus type 1 (HIV-1) is a routine component of
clinical management, and there are now many classification
algorithms available for this purpose. 

**Ours is an alignment-free subtyping method using Recurrent
Neural Networks (RNN) that operates on both time series analysis of the
individual character and k-mer frequencies in HIV-1 sequences.**


## Dataset Description
- The dataset is taken from
https://www.hiv.lanl.gov/components/sequence/HIV/search/
185search.html
- The dataset consists of 243 subtypes of HIV-1 genomes. We
had a total of 12,938 sample genomes, with these 243
subtypes. We took 25 subtypes among them, which consisted of the
heighest samples. The subtype with heighest samples was ’B’, with 5727
samples. And the subtype ’35 AD’, with 22 samples.

## Model Summary
![Model Summary](https://github.com/nishatbristy007/HIV-1-subtype-classification/blob/main/model_summary.png)

## Results
![Results](https://github.com/nishatbristy007/HIV-1-subtype-classification/blob/main/results.JPG)

**A few takes on the results**
- Our observation is that with character level time-series analysis, a sliding window approach seems to be the most accurate.  This is because sliding window gives the opportunity of increasing samples in the training dataset, as well as ensures that every portion and functional relation of the genome is being considered.
- For k-mer analysis, both k = 15 and k = 21 performs significantly good.

## Data Availability

The project is available at [Google Drive](https://drive.google.com/drive/folders/1QAbltLllvnhrpkOtDHLPdKGmP6j0UQId?usp=sharing)

A brief presentation is available at [this link](https://github.com/nishatbristy007/HIV-1-subtype-classification/blob/main/HIV-1%20Subtyping%20Using%20RNN%20(Slides).pdf).

The web application [Link](https://mm7yg5x64d2ce5ht.anvil.app/KVWNR77PLK47F3XLHLJ5PTJB) (Note that the server needs to be running for this link to work.)
