# PPQM todo-list
For desired every capability add a bullet point, with sub-bullet points with references and where to steal code


## NDDO/MNDO capabilities:

* Analytical implementation of overlap integrals
  * https://github.com/matthiaslein/WellFARe-STO/blob/master/wellfareSTO.py
* Analytical implementation of MNDO two-electron integrals
  * MiniAMBER code
* Fock-matrix assembly
  * Should be easy to write
* Exact diagonalization (LAPACK) and pseudo-diagonalization
  * Exact diagonalizer from MKL or LibElemental, pseudo diagonalizer from AMBER?
* _Stable_ SCF convergers (Quadratic, DIIS, etc)
  * ??
* Analytical first derivative (i.e. gradient)
  * ??
* (Analytical Hessian?)
  * ??

## DFTB capabilites:
* Slater-Koster file parser
  * AMBER 
* Integral rotations
  * AMBER 
* Fock-matrix assembly
  * Should be easy to write
* Mixers (Anderson/DIIS/Broyden)
  * ??
* Analytical first derivative (i.e. gradient)
  * ??
* (Analytical Hessian?)
  * ??

## Optimizer:
* Find out which optimizer is used in Gaussian, Gamess, etc
  * ??

## Solvent:
* PCM (which version?)
  * ??
* COSMO/COSMO-RS
  * ??
