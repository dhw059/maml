<img src="https://github.com/materialsvirtuallab/maml/blob/master/resources/logo_horizontal.png?raw=true" alt="maml" width="50%">

[![GitHub license](https://img.shields.io/github/license/materialsvirtuallab/maml)](https://github.com/materialsvirtuallab/maml/blob/main/LICENSE)
[![Linting](https://github.com/materialsvirtuallab/maml/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/maml/workflows/Linting/badge.svg)
[![Testing](https://github.com/materialsvirtuallab/maml/workflows/Testing/badge.svg)](https://github.com/materialsvirtuallab/maml/workflows/Testing/badge.svg)
[![Downloads](https://pepy.tech/badge/maml)](https://pepy.tech/project/maml)
[![codecov](https://codecov.io/gh/materialsvirtuallab/maml/branch/master/graph/badge.svg?token=QNL1CRLVVL)](https://codecov.io/gh/materialsvirtuallab/maml)

maml (MAterials Machine Learning) is a Python package that aims to provide useful high-level interfaces that make ML
for materials science as easy as possible.

The goal of maml is not to duplicate functionality already available in other packages. maml relies on well-established
packages such as scikit-learn and tensorflow for implementations of ML algorithms, as well as other materials science
packages such as [pymatgen](http://pymatgen.org) and [matminer](http://hackingmaterials.lbl.gov/matminer/) for
crystal/molecule manipulation and feature generation.



# Features

1. Convert materials (crystals and molecules) into features. In addition to common compositional, site and structural
   features, we provide the following fine-grain local environment features.

 a) Bispectrum coefficients
 b) Behler Parrinello symmetry functions
 c) Smooth Overlap of Atom Position (SOAP)
 d) Graph network features (composition, site and structure)

2. Use ML to learn relationship between features and targets. Currently, the `maml` supports `sklearn` and `keras`
   models.

3. Applications:

 a) `pes` for modelling the potential energy surface, constructing surrogate models for property prediction.

  i) Neural Network Potential (NNP)
  ii) Gaussian approximation potential (GAP) with SOAP features
  iii) Spectral neighbor analysis potential (SNAP)
  iv) Moment Tensor Potential (MTP)

 b) `rfxas` for random forest models in predicting atomic local environments from X-ray absorption spectroscopy.

 c) `bowsr` for rapid structural relaxation with bayesian optimization and surrogate energy model.

# Installation

Pip install via PyPI:

```bash
pip install maml
```

To run the potential energy surface (pes), lammps installation is required you can install from source or from `conda`::

```bash
conda install -c conda-forge/label/cf202003 lammps
```

The SNAP potential comes with this lammps installation. The GAP package for GAP and MLIP package for MTP are needed to run the corresponding potentials. For fitting NNP potential, the `n2p2` package is needed.

Install all the libraries from requirement.txt file::

```bash
pip install -r requirements.txt
```

For all the requirements above::

```bash
pip install -r requirements-ci.txt
pip install -r requirements-optional.txt
pip install -r requirements-dl.txt
pip install -r requirements.txt
```

# Usage

Many Jupyter notebooks are available on usage. See [notebooks](/notebooks). 

# API documentation

See [API docs](https://materialsvirtuallab.github.io/maml/maml.html).

# Citing

```txt
Graph neural networks-based transfer learning framework for enhanced predictive performance on diverse small and large materials datasets
```


