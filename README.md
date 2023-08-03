# atomman-demo

This repository provides an introductory overview for the various resources and tools created by the NIST Interatomic Potentials Repository project.  This is not meant to provide comprehensive documentation for all parts of the project as those are available elsewhere.  Links to the more in-depth docs can be found throughout the contents of this repository.

## Documentation content

- [1. Introduction.md](https://github.com/lmhale99/atomman-demo/blob/main/1.%20Introduction.md) offers an overview of the NIST Interatomic Potentials Repository resources and tools.
- [2. Basics of atomman.ipynb](https://github.com/lmhale99/atomman-demo/blob/main/2.%20Basics%20of%20atomman.ipynb) gives a step-by-step overview of how atomman can be used to select an interatomic potential, generate an atomic configuration, set up and run a LAMMPS simulation, and access the results for further processing and analysis.

## Interactive content

The Basics of atomman Notebook is designed both to provide documentation and the means for users to interact with the different methods and behaviors.  To run the Notebook for yourself, you can either open it in colab or download it locally.

### Google colab

If you have a google account, you can run the Notebook in colab without needing to install anything.  This provides a simple
way of trying out some of the features of atomman.

- Colab link for [2. Basics of atomman.ipynb](https://colab.research.google.com/github/lmhale99/atomman-demo/blob/main/2.%20Basics%20of%20atomman.ipynb)

### Download and install

You can also download and install atomman and this git repository and try out the Notebooks yourself.

1. Install Python if needed.  Anaconda distributions are recommended (especially for windows users), but regular Python will work as well as long as it is version 3.7+.
2. Optional: If you already have anaconda, you can create a new environment if you are worried about any package conflicts.
3. Download or clone this repository to a local directory.
4. Install atomman as described at the top of the Notebook.

## Supporting content in this repository

- lmp.gz is a zipped LAMMPS executable that was built in colab.  Notebooks running in colab can download this file to run LAMMPS simulations.
- make_lammps_for_colab.ipynb creates the lmp.gz file for the current version of LAMMPS.
- run/ contains the LAMMPS output files for an example run of the Basics of atomman Notebook.  This makes it possible to interact with the LAMMPS outputs without needing to run LAMMPS again.
- images/ contains the pictures that are seen in the Introduction Notebook.
