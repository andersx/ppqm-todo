# PPQM todo-list
For desired every capability add a bullet point, with sub-bullet points with references and where to steal code

## PPQM capabilities

* Python Bindings
   * All modules easily portable as standalone, for easy python bindings
   
* One-executable
   * For normal use and non-experts, use one executable with a input file
 
## NDDO/MNDO capabilities:

* Analytical implementation of overlap integrals
  * https://github.com/matthiaslein/WellFARe-STO/blob/master/wellfareSTO.py
* Analytical implementation of MNDO two-electron integrals
  * MiniAMBER code
* Fock-matrix assembly for NDDO, CNDO, MNDO, AM1/PM3/PM6/PM7, etc
  * Should be easy to write (just to clarify, Andersx wrote that. Famous last words)
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

## Corrections:
* Dispersion D3
  * Stefan Grimme
* H+
  * Jimmy's kode

## Optimizer:
* Find out which optimizer is used in Gaussian, Gamess, etc
  * ??
* TS optimizer:
  * GSM
  * Optimize to transition state (e.g. QST2/QST3)?

## Solvent:
* PCM (which version?)
  * ??
* COSMO/COSMO-RS
  * ??
  
## Fragmentation:
* Which scheme?
  * FMO?
  * Linear-scaling sparse matrix?

