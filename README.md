# FEMxHE: Finite Element Method for Heat Equation

## Overview

This repository contains the code used for a number of examples regarding heat diffusion problems. It is made public, for everyone to be able to reproduce the results of the proposed examples, for which we provide Python Jupyter notebooks. Each problem's solution is given through numerical methods, specifically using the Finite Element Method (FEM). The implementation relies on the FEniCS library.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Dependencies](#dependencies)
- [License](#license)

## Installation

In order to run the proposed examples, start by cloning this repository

```bash
# Clone the repository
git clone https://github.com/leobcc/FEMxHE.git
cd FEMxHE
```
Then you will need to install the necessary DOLPHINx environment, including the FEniCSx library. For the installation, you can refer to their page https://github.com/FEniCS/dolfinx, on which they propose different methods to proceed. In our case, we use the docker image containing a Jupyter Lab environment with the latest stable release of DOLFINx

```bash
docker run --init -ti --gpus all --name fenicsx -p 8888:8888 -v "${PWD}:/root/FEMxHE" dolfinx/lab:stable
```
Now the environment should be set up correctly, and it should be possible to run the Jupyter notebooks effortlessly from within the docker container.

## Dependencies

The dependencies are numerous but they coincide with the ones of the computational environment DOLFINx. Hence, by using the docker image of the last stable version of DOLFINx as a base image, the user should not have to handle particular dependencies or install/update additional libraries.  

## Usage

To reproduce the results of the examples, no further particular action is needed. Each example is studied and solved in its dedicated Jupyer notebook, so that the results are easily reproducible by simply going through the notebook itself.

## License

This project is licensed under the [MIT License](LICENSE.md) - see the [LICENSE.md](LICENSE.md) file for details.
