# Comparison Results of Primal and Mixed Finite Element Methods for the Darcy problem 
### NUMERICAL ANALYSIS FOR PARTIAL DIFFERENTIAL EQUATIONS 
#### *Politecnico di Milano* (ITALY)
**Prof.**  : Simona Perotto

**A.Y.**   : 2014-2015

**Author** : Domenico Notaro (ID 10332103)

**Mailto** : <domenico.not@gmail.com>

-------------------------------------------------------

A finite element solver written in [*FreeFem++*](http://www.freefem.org/).

It simulates the Darcy flow in porous media (see `report.pdf` for mathematical details).

--------------------------------------------------------
## Code organization

- `assembling.edp` : 
- `fem.edp`        :
- `macros.edp`     :
- `main.edp`       :
- `mesh.edp`       :

--------------------------------------------------------
## Execution
Before running the main program you have to set the desired framework.
1. Define a computational mesh in `mesh.edp`
-> set the number of subdivisions
2. Select the FE approximation in `fem.edp` 
-> Uncomment the desired method (Lagrange, Croizeuix-Raviart, Raviart-Thomas, ...) 
3. Run the program
``` 
$ FreeFem++ main.edp
``` 
