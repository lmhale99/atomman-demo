# atomman-demo

This repository provides demonstration Notebooks for the atomman Python package.

## Option #1: colab

If you have a google account, you can run the first two Notebooks in colab without needing to install anything.  This provides a simple, lightweight
way of trying out some of the features of atomman.

Colab link for [1. Interatomic Potentials.ipynb](https://colab.research.google.com/github/lmhale99/atomman/blob/master/1.%20Interatomic%20Potentials.ipynb)
Colab link for [2. Atomic Systems.ipynb](https://colab.research.google.com/github/lmhale99/atomman/blob/master/2.%20Atomic%20Systems.ipynb)

The "3. LAMMPS runs.ipynb" performs LAMMPS simulations, so it would require a simple means of installing LAMMPS for colab...

## Option #2: Download and install

You can also download and install atomman and this git repository and try out the Notebooks yourself.

1. Install Python if needed.  Anaconda distributions are recommended (especially for windows users), but regular Python will work as well as long as it is version 3.7+.
2. Optional: If you already have anaconda, you can create a new environment if you are worried about any package conflicts.
3. Install atomman.  If you are using anaconda, then use "conda install -c conda-forge atomman".  Otherwise "pip install atomman". 
4. Download or clone this repository.