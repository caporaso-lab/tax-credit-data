# TAX CREdiT data: TAXonomic ClassifieR Evaluation Tool data repository

### A standardized and extensible evaluation framework for taxonomic classifiers

This repository contains all data and Jupyter notebooks for the tax-credit project, a standardized and extensible evaluation framework for assessing short-read taxonomic classifiers.

To view static versions of the reports, [start here](https://github.com/caporaso-lab/tax-credit-data/blob/master/ipynb/Index.ipynb).

Environment
-----------------
This repository contains Python 3 Jupyter notebooks, but some taxonomy assignment methods (e.g., using QIIME-1 legacy methods) may require different python or software versions. Hence, we use conda parallel environments to support comparison of myriad methods in a single framework.

The first step is to install conda and install QIIME2 following the instructions provided [here](https://docs.qiime2.org/2017.6/install/native/).

An example of how to load different environments to support other methods can be seen in the [QIIME-1 taxonomy assignment notebook](https://github.com/caporaso-lab/tax-credit-data/blob/master/ipynb/mock-community/taxonomy-assignment-qiime1.ipynb).


Setup and install
-----------------
To clone this repository:
```
git clone https://github.com/caporaso-lab/tax-credit-data.git
```

The tax-credit python 3 package is hosted in the [tax-credit-code repository](https://github.com/caporaso-lab/tax-credit-code).

```
git clone https://github.com/caporaso-lab/tax-credit-code.git
cd tax-credit-code
pip install .
```

OR

```
pip install https://github.com/caporaso-lab/tax-credit-code/archive/master.zip
```

To extend the 16S/ITS classification results you will need reference data sets:

```
wget https://unite.ut.ee/sh_files/sh_qiime_release_20.11.2016.zip
wget ftp://greengenes.microbio.me/greengenes_release/gg_13_5/gg_13_8_otus.tar.gz
unzip sh_qiime_release_20.11.2016.zip
tar -xzf gg_13_8_otus.tar.gz
```


Using the Jupyter Notebooks included in this repository
-------------------------------------------------------

To view and interact with [Jupyter Notebook](http://jupyter.org/), change into the ``/tax-credit-data/ipynb`` directory and run Jupyter Notebooks from the terminal with the command:

``jupyter notebook index.ipynb``

The notebooks menu should open in your browser. From the main index, you can follow the menus to browse different analyses, or use ``File --> Open`` from the notebook toolbar to access the full file tree.


Citing
------

If you use any of the data or code included in this repository, please cite:

Bokulich NA, Kaehler BD, Rideout JR, Dillon M, Bolyen E, Knight R, Huttley GA, Caporaso JG. (2017) Optimizing taxonomic classification of marker gene sequences with QIIME 2's q2-feature-classifier. Microbiome 6:90 https://doi.org/10.1186/s40168-018-0470-z
