# A Hybrid Matrix Factorization via Graph SignalProcessing

## Abstract
Predicting whether a user would like a particular item has become significantly important for the success of commercial applications like Netflix, YouTube, Spotify, etc.
One of the techniques that has become predominant for this task is formulating the problem as a matrix factorization one and trying to explain each rating as a numerical representation of the corresponding user and item.
However, it is a standard problem that could be optimized with stochastic gradient descent (SGD) and there is no novelty in that approach.

In this project, we try to extend this approach by utilizing well known techniques from graph signal processing.
The extension is consisted of two parts: 1) utilizing graph Fourier transform to switch from vertex graph domain to spectral graph domain, and 2) applying graph filters to denoise the obtained features.
Using these techniques we have achieved an improvement of 4% over our baseline model -- the standard matrix factorization technique with SGD.


## Project Structure
The project is organized as follows:

    .
    ├── read_the_data.ipynb             # Jupyter Notebook for exploring the dataset
    ├── main.ipynb                      # A clear Jupyter Notebook which can be used for new testings
    ├── main_results.ipynb              # Jupyter Notebook that has the run models, and the figures used in the report
    ├── oimdb_metadata_crawled.pickle   # Open Movie Database (OMDb) crawled data
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
- networkx
```

## License
This project is licensed under the terms of the MIT license.

## Authors

* Ljupche Milosheski    ljupche.milosheski@epfl.ch
* Alen Carin            alen.carin@epfl.ch
* Blagoj Mitrevski      blagoj.mitrevski@epfl.ch
* Mladen Korunoski      mladen.korunoski@epfl.ch
