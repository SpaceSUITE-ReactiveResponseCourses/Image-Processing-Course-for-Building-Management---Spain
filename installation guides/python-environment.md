# UHI Project – Conda Environment Setup

This document explains how to create and configure a working Python environment for the UHI project using Miniconda.

It is recommended to put your project folder in your drive root, or in Documents. In this example, we will use D:\

---

## 1. Open Miniconda

Open your **Miniconda Prompt** (Windows) or **Terminal** (macOS / Linux).

Navigate to your UHI project folder:


cd D:\UHI

## 2. Create and Activate the Conda Environment

Create the environment _inside the project folder_:

`conda create --prefix ./uhi-env` 

`conda activate ./uhi-env`

---
## 3. Install Required Python Packages
Run the following lines on your terminal in this order: 

i) `conda install geopandas localtileserver ipykernel jupyterlab earthengine-api -c conda-forge`

ii) `conda install geemap -c conda-forge` 

iii) `pip install oeel`

---

## 4. Install Node.js (required for OEEL)

`conda install nodejs=18.17.1`

---

## 5. Install Required npm Packages for OEEL

Navigate to the OEEL package directory:

`cd ./uhi-env/Lib/site-packages/oeel`

Install npm dependencies:

`npm install zeromq@6.0.0-beta.6 unpromisefy`

---

## 6. Usage Notes

To activate the environment later within your project folder:

`conda activate ./uhi-env`

To deactivate the environment:

`conda deactivate`
