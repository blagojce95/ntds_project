# A Hybrid Matrix Factorization via Graph SignalProcessing

## Abstract
Successfully predicting what rating a user would give to a particular item has become significantly important for the success of commercial applications such as Netflix, YouTube, Spotify, and many others.
One of the techniques that has become predominant for this task is formulating the problem as a matrix factorization one and trying to explain each rating as a numerical representation of the corresponding user and item.

In this project, we try to extend this approach by utilizing well known techniques from graph signal processing.
The extension is consisted of two parts: 1) utilizing graph Fourier transform to switch from vertex graph domain to spectral graph domain, and 2) applying graph filters to denoise the obtained signals.
Using these techniques we have achieved an improvement of \textbf{TODO}\% over our baseline model, the regular matrix factorization.


## Project Structure
The project is organized as follows:

    .
    ├── read_the_data.ipynb             # Jupyter Notebook for exploring the dataset
    ├── main_standard_matrix_fact.ipynb # Jupyter Notebook for the baseline model
    ├── main_gft.ipynb                  # Jupyter Notebook for the our hybrid approach
    ├── oimdb_metadata_crawled.pickle   # Open Movie Database (OMDb) crawl 
    └── ml-100k                         # MovieLens 100k dataset


## Prerequisites
The project was created and tested with the following dependencies:

### Libraries
```
- Anaconda Python 3.6.5
- pickle
- numpy
- pandas
- sklearn
- matplotlib
```

## License
This project is licensed under the terms of the MIT license.

## Authors

* Ljupche Milosheski    ljupche.milosheski@epfl.ch
* Alen Carin            alen.carin@epfl.ch
* Blagoj Mitrevski      blagoj.mitrevski@epfl.ch
* Mladen Korunoski      mladen.korunoski@epfl.ch
