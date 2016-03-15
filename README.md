# Comparison Results of Primal and Mixed Finite Element Methods for the Darcy problem 
### NUMERICAL ANALYSIS FOR PARTIAL DIFFERENTIAL EQUATIONS 
#### *Politecnico di Milano* (ITALY)

**Author** : Domenico Notaro (ID 10332103)

**Mailto** : <domenico.not@gmail.com>

**Date**   : March 2016

-------------------------------------------------------

A finite element solver written in [*FreeFem++*](http://www.freefem.org/) (version 3.45, Ubuntu 14.04).

It simulates the Darcy flow in porous media (see `report.pdf` for mathematical details).

Different finite element methods are provided, both in primal and mixed form.

--------------------------------------------------------
## The Code
The package is organized as follows:

- `assembling.edp` : definition of the primal and mixed variational problems
- `fem.edp`        : list of available finite element methods
- `macros.edp`     : definition of useful macros
- `main.edp`       : main program to compare the primal and mixed solutions
- `mesh.edp`       : generatation of the computational mesh

--------------------------------------------------------
## Execution
Before running the main program you have to set the desired framework.

1. Define a computational mesh in `mesh.edp` (number of subdivision)
2. Select the FE approximation in `fem.edp` (Lagrange, Croizeuix-Raviart, Raviart-Thomas, ...) 
3. Run the program
``` 
$ FreeFem++ main.edp
``` 
