# xarray-tutorial

[![Build](https://github.com/andersy005/xarray-tutorial/actions/workflows/build.yml/badge.svg)](https://github.com/andersy005/xarray-tutorial/actions/workflows/build.yml)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/andersy005/xarray-tutorial/main?urlpath=lab)

This repository contains materials for the xarray tutorial.

## Running the tutorial

There are two different ways in which you can set up and go through the tutorial materials. Both of which are outlined in the table below.

|    Method     |                                                          Setup                                                           | Description                                                                                                                                                                                                             |
| :-----------: | :----------------------------------------------------------------------------------------------------------------------: | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|    Binder     | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/andersy005/xarray-tutorial/main?urlpath=lab) | Run the tutorial notebooks on mybinder.org without installing anything locally.                                                                                                                                         |
| Local install |                                     [Instructions](#Local-installation-instructions)                                     | Download the tutorial notebooks and install the necessary packages (via `conda`) locally. Setting things up locally can take a few minutes, so we recommend going through the installation steps prior to the tutorial. |

## Local installation instructions

### 1. Clone the repository

First clone this repository to your local machine via:

```
git clone https://github.com/andersy005/xarray-tutorial
```

### 2. Download conda (if you haven't already)

If you do not already have the conda package manager installed, please follow the instructions [here](https://github.com/conda-forge/miniforge#install).

### 3. Create a conda environment

Navigate to the `xarray-tutorial/` directory and create a new conda environment with the required
packages via:

```terminal
cd xarray-tutorial
conda env update --file binder/environment.yml
```

This will create a new conda environment named "xarray-tutorial".

### 4. Activate the environment

Next, activate the environment:

```
conda activate xarray-tutorial
```

### 5. Download sample datasets

To download sample datasets, run the `00-download-data.ipynb` notebook:

```bash
cd notebooks/
nbterm --run 00-download-data.ipynb
```

### 6. Launch JupyterLab

Finally, launch JupyterLab with:

```
jupyter lab
```
