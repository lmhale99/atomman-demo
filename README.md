# atomman-demo

This repository provides a quick introductory overview for the various resources and tools created by the NIST Interatomic Potentials Repository (IPR) project.  This is not meant to provide comprehensive documentation for all parts of the project as those are available elsewhere.  Links to the more in-depth docs can be found throughout the contents of this repository.

## Setup for this demo

1. Install LAMMPS.  If you are building LAMMPS yourself, create a LAMMPS executable. 
2. Install Python if needed.  Optionally, if you are using conda you can create a new environment to avoid any possible package conflicts.
3. Download or clone this repository to a local directory.
4. Install iprPy using either "pip install iprPy" or "conda install -c conda-forge iprPy"


## Notebook overview

- __1. Find and interact with LAMMPS potentials and crystals__ gives the basics for how interatomic potentials and any associated relaxed crystal structures can be easily found and accessed from the IRP database. 
- __2. Basics of atomman__ gives a quick overview of building and manipulating atomic configurations in Python using atomman.
- __3. Run LAMMPS with atomman__ shows how to set up and run LAMMPS simulations that take advantage of the tools mentioned in the first 2 Notebooks.
- __4. iprPy calculation basics__ outlines how to access and run any of the calculations currently implemented in iprPy, and how to explore results from finished calculations.
- __5. High throughput workflow example__ provides an example of using the high throughput workflow tools to run many calculation instances.