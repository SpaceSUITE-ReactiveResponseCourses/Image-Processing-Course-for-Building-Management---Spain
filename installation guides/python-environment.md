# UHI Project – Conda Environment Setup

This document explains how to create and configure a working Python environment for the UHI project using Miniconda.

All the lines provided in `this format` are to be copied and pasted onto you terminal, and press ENTER to run them, in the order provided.

It is recommended to put your project folder/save the UHI folder provided in your drive root, preferrably outside of C:\. In this example, we will use D:\

**NOTE**: While installing conda and the packages, please keep an eye on your terminal for **Proceed([y]/n)?** prompts, and type in **y** to continue.

---

## 1. Open Miniconda

#### **Windows**
1. Click the **Start Menu**.
2. Type **Miniconda**.
3. Select **Miniconda Prompt** (or **Anaconda Prompt(Miniconda3** ).
4. A command window opens — this is where you will enter conda commands.

#### **macOS**
1. Open **Finder**.
2. Go to **Applications → Utilities**.
3. Open **Terminal**.
4. You can now type conda commands — but if conda is not recognized yet, run:
    `source ~/.zshrc`

#### **Linux (Ubuntu/Debian)**
1. Press **Ctrl + Alt + T** to open Terminal, or open **Terminal** from your applications menu.
2. Type conda commands — if conda is not recognized, run:
    `source ~/.bashrc`
    (or `source ~/.zshrc` if using zsh)

---

## 2. Create and Activate the Conda Environment

`conda create -n uhi-env python=3.11` 

`conda activate uhi-env`

---
## 3. Install Required Python Packages

Copy and paste the following lines on your terminal, and run(press enter): 

`conda install geemap geopandas localtileserver ipykernel jupyterlab earthengine-api nb_conda_kernels -c conda-forge`

---

## 6. Usage Notes

To activate the environment later within your project folder:

`conda activate uhi-env`

To deactivate the environment:

`conda deactivate`


You can close your terminal
