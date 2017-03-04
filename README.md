# PPQM todo-list
For desired every capability add a bullet point, with sub-bullet points with references and where to steal code

## PPQM capabilities

* Python Bindings
   * All modules easily portable as standalone, for easy python bindings
   
* One-executable
   * For normal use and non-experts, use one executable with a input file
   
* Improved parametrization for biomolecules and drugs
 
## Check of Semiempirical approximation
 * Step one is reparametrization of available SQM methods using *existing* dataset of MP2 heat-of-formation for GDB7, GDB8 or GDB9 datasets. We aim to re-parametrize the following methods:
   * MNDO - the baseline method
   * MNDO/d - MNDO with d-orbitals
   * MNDOC - MNDO with BWEN perturbation theory correlation term
   * AM1 - MNDO with additional core-repulsion terms
   * PM6 - Same as AM1, but pairwise core-repulsion terms http://openmopac.net/Manual/external.html
   * OMx - Orthogonalization corrected method
   * Modified OMx - Disable orthogonalization correction and compare effect of gaussian/ECP integrals with MNDO multipole integrals.
 
## NDDO/MNDO capabilities:

* Analytical implementation of overlap integrals
  * https://github.com/matthiaslein/WellFARe-STO/blob/master/wellfareSTO.py
* Analytical implementation of MNDO two-electron integrals
  * MiniAMBER code
* Fock-matrix assembly for NDDO, CNDO, MNDO, AM1/PM3/PM6/PM7, etc
  * Should be easy to write (just to clarify, Andersx wrote that. Famous last words)
  * RHF and UHF type wave functions
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
  * Spin-polarized/open-shell DFTB
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
* Use Python optimizers (with fortran bindings) to test different optimizers


## Solvent:
* PCM (which version?)
  * ??
* COSMO/COSMO-RS
  * ??
  
## Fragmentation:
* Which scheme?
  * FMO?
  * Linear-scaling sparse matrix?

## Parametrization:
* Review of semiempirical approximations
  * https://www.overleaf.com/read/rdrcfqpckpbk
* Construction of dataset from CCSD(T)
  * Identify relevant molecules from ZINC database or GDB\* database
  * Heats-of-formation dataset
  * Non-covalent interactions dataset
  * Reaction barriers
  * Rotational barriers
