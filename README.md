# Grayskull
-------------
[![Build Status](https://dev.azure.com/marceloduartetrevisani/Grayskull/_apis/build/status/Tests?branchName=master)](https://dev.azure.com/marceloduartetrevisani/Grayskull/_build/latest?definitionId=4&branchName=master) [![codecov](https://codecov.io/gh/marcelotrevisani/grayskull/branch/master/graph/badge.svg)](https://codecov.io/gh/marcelotrevisani/grayskull) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) ![](https://img.shields.io/badge/python-3.7+-blue.svg) ![](https://img.shields.io/github/license/marcelotrevisani/grayskull.svg)

-------------
![Grayskull](https://comicvine1.cbsistatic.com/uploads/original/4/49448/2661756-castle_grayskull.jpg)

*"Skeleto~~n~~r's main goal is to conquer the mysterious fortress of Castle Grayskull, from which He-Man draws his powers. If he succeeds, Skeletor would be able to conquer not only Eternia, but the whole universe."* Adapted from [Wikipedia](https://en.wikipedia.org/wiki/Skeletor)
-------------
## Introduction

The Grayskull project was created with the intention to eventually replace the
`conda skeleton`. The main goal of this project is to generate concise recipes
 for [conda-forge](https://conda-forge.org/).

The current status of ``grayskull`` is generating recipes just looking for ``PyPI``,
 but in the future we will expand that to also support to load recipes and also
 generate recipes looking for other repositories, such as, CRAN, Conan, etc..

## Installation

It is possible to install this project using `pip`:
```bash
pip install grayskull
```

or `conda`, using the ``conda-forge`` channel:
```bash
conda install -c conda-forge grayskull
```

It is also possible to clone this repo and install it using `pip`:
```bash
git clone https://github.com/marcelotrevisani/grayskull.git
cd grayskull
pip install -e .
```

## Usage

It is pretty simple to use `grayskull`. Just call it, pass the repository
 (just `pypi` for now) and the package name.

* Example:
```bash
grayskull pypi pytest
```

After that `grayskull` will create a folder with the same name as the package
and inside of this folder it will generated the recipe (`meta.yaml`).

* Example with `pytest` (`grayskull pypi pytest`):

![Grayskull CLI](docs/images/cli_example_grayskull.gif)


## License
Copyright Marcelo Duarte Trevisani and others, 2020-2021.

Distributed under the terms of the MIT license, grayskull is free and open source software.
