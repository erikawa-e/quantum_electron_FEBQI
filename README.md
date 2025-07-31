# Environment Setup Instructions (Python 3.13.3 + quantum_electron_FEBQI)

This guide explains how to create a Conda virtual environment named `qe_thomas`, clone the `quantum_electron_FEBQI` repository (on the `thomas` branch), and install the required packages.

## 1. Create and activate the Conda environment

First, create a new environment using Python 3.13.3 and activate it:

```bash
conda create -n qe_thomas python=3.13.3
conda activate qe_thomas
```

---

## 2. Clone the repository (`thomas` branch)

Clone the repository using the `thomas` branch:

```bash
git clone --branch thomas git@github.com:erikawa-e/quantum_electron_FEBQI.git
```

---

## 3. Install the main `quantum_electron` package (editable mode)

Navigate into the repository and install the main package in editable mode:

```bash
cd quantum_electron_FEBQI
cd quantum_electron
pip install -e .
```

> The `-e` option installs the package in "editable" mode, so any code changes take effect immediately.

---

## 4. Install `zeroheliumkit` dependencies and register the package

Navigate to the `zeroheliumkit` subdirectory, install its dependencies, and register the package in editable mode:

```bash
cd zeroheliumkit
pip install -r requirements.txt
pip install -e .
```

---

## ✅ Installation Done

Your Python environment is now ready for development and running the code.

Run
quantum_electron_FEBQI/thomas_simulations/resevoir_sample.ipynb

quantum_electron_FEBQI/thomas_simulations/sim_test/sample_resevoir_10x10_no_bond_lines.dxf
is the geometry of our sample.

<img width="951" height="656" alt="image" src="https://github.com/user-attachments/assets/eac47702-ca57-49fd-b3bb-12f07efec4db" />

<img width="304" height="471" alt="image" src="https://github.com/user-attachments/assets/9124bc47-41e1-4637-a4b8-12f3b43c91f0" />


##
Run
thomas_simulations/resevoir_sample.ipynb

Run 
thomas_simulations/unloading_new_Guard.ipynb
or
thomas_simulations/unloading_new_one_gates.ipynb

