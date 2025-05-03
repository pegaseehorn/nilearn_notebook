---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.11.5
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

We can either run the code locally with Python installed on our own machine, or utilise the universities' High Performance Cluster. Two options are described in this Jupyter Notebook.


# Setup coding environment

If you decide to run the code locally you can follow the guide here:
For easy coding environment management we can use Anaconda / miniconda.

You should have the following programmes installed:

- Anaconda (miniconda)
- Code editor (e.g. Visual Studio code, Spyder)

If not, please follow the installation instructions from the [psy111](https://mibur1.github.io/psy111/book/introduction/1_Setup/0_Introduction.html) module by Micha Burkhard.

<br >
<br >

We start by setting up a new conda environment for using NiLearn. 

In the Miniconda prompt let's first ensure that we install the necessary dependencies from an up-to-date and reliable source. We’ll do this by adding the conda-forge channel and setting it as the default with strict priority.

```bash
conda config --add channels conda-forge
```
```bash
conda config --set channel_priority strict
```

<br >
<br >

Now we can create a new Conda environment and activate it:


```bash
conda create -n NiLearn python
```
```bash
conda activate NiLearn
```

If the environment now shows up as `(NiLearn)`, you are ready to install the required Python packages for using NiLearn:

```bash
pip install nilearn
```

## HPC option
Preferably, we use the high performance cluster (HPC) to run our code. The notebook for today is plit into different chapters for easy explanation and organisation. But, this also makes it tedious to upload and use the code on the HPC. So, for that you can use the unified code version that you can find in the table of contents under 'HPC version'.

1. Upload this code to the HPC via
2. Open Neurodesk on the HPC.
3. Use Neurodesk to open and run this Jupyter Notebook.