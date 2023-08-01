# Getting Interatomic Potentials from the NIST Interatomic Potentials Repository

The NIST Interatomic Potentials Repository serves as host for community-developed interatomic potentials that primarily focus on representing crystalline materials. The project aims to make it easy for users to discover, download, compare and use existing classical interatomic potentials.

## 1. Interatomic Potentials Repository

The Interatomic Potentials Repository is a website that can be visited at https://www.ctcms.nist.gov/potentials/.

![Interatomic Potentials Repository homepage](./images/ipr-homepage.png)

- - -

If you click on an element or elemental system, it will bring up a list of all hosted interatomic potentials that offer models for that element. Each listing can provide the following information
- Each potential has a unique ID.
- Citation information including abstract(s).
- A list of related models that share the same or nearly the same interactions.
- General usage notes about the potential, such as what it was originally designed for.
- A list of known hosted implementations.
    - Each implementation has a unique ID.
    - Notes on where the files originated and any conversion/validation notes if needed.
    - Downloadable links to the parameter files and/or web links to external sites where the content is hosted.
    - For LAMMPS-compatible potentials, a "See Computed Properties" link to view computed properties.    

![Interatomic Potentials Repository entry example](./images/ipr-entry.png)

- - -

Clicking on the "See Computed Properties" link for an implementation will open a page with a list of all current computed properties and descriptions of the methodologies used.

![Interatomic Potentials Repository elastic constants example](./images/ipr-cij.png)

## 2. CDCS database of potentials

Alternatively, the content hosted by the Interatomic Potentials Repository can be explored from the underlying CDCS database hosted at https://potentials.nist.gov/

![CDCS potentials.nist.gov homepage](./images/cdcs-homepage.png)

- - -

The easiest way to explore the content is to select "Data Exploration->Search By Keyword" from the top bar. Then, you can select one or more record templates on the left and enter any keywords in the search bubble to look for.

The database has many different templates for representing different content.  The ones most likely of interest to users are 

- __Potential__ provides the listings of interatomic potentials as they appear on the main Repository website.
- __potential_LAMMPS__ provides metadata associated with the LAMMPS implementations of the potentials. These are used by the supporting Python packages to make it possible to download parameter files and generate LAMMPS input commands for a potential.
- __potential_LAMMPS_KIM__ provides metadata associated with running different KIM models in LAMMPS and how they are connected to the Potential listings.
- __crystal_prototype__ give structure information for a limited number of crystal prototypes.
- __relaxed_crystal__ give structure information for crystal structures relaxed with a specific interatomic potential.
- __PotentialProperties__ lists the processed calculation data for the computed properties on the main Repository website. (Limited to raw XML only at the moment)
- __calculation\_\*__ templates are the raw results records for individual calculation runs.  The available set of calculation types is gradually being increased.

![CDCS potentials.nist.gov search](./images/cdcs-search.png)

## 3. GitHub archive of records

There is also a GitHub repository that serves as an archive of many of the records in the database.  This GitHub repository can be found at https://github.com/lmhale99/potentials-library.  This repository includes copies of all parameter files for LAMMPS-compatible potentials as well as the records associated with the website and input parameter sets.  The downsides to getting the files from the GitHub repository are that it tends to get updated 1-2 times a year, all records are in JSON so an interpreter is needed, and it only includes content for the potentials listings and some other input content.

![potentials-library github repository](./images/github.png)

## 4. Python packages

The Interatomic Potentials Repository provides a number of Python packages that are designed to interact with the database records.  The main packages are

- __potentials__ (https://github.com/usnistgov/potentials) provides APIs for interacting with the potential-related records in the https://potentials.nist.gov/ database.
- __atomman__ (https://www.ctcms.nist.gov/potentials/atomman/) includes all APIs from potentials plus methods and tools for generating, manipulating and analyzing atomic configurations.
- __iprPy__ (https://www.ctcms.nist.gov/potentials/iprPy/) contains a collection of complete property calculation scripts and high throughput tools 
