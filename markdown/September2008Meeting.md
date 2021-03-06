This talk will be an introduction to doing scientific computing with Perl and Math::GSL.

* features:
  * numerical derivatives and integration
  * special functions, statistics, permutations/combinations
  * random number generators
  * Linear algebra (BLAS)
  * Fast Fourier Transform
  * Wavelets
  * Splines/Interpolation
  * Histograms
  * 1D Curve Fitting
  * 1D Root Solving 
  * Multidim. Root Solving (soon)
  * Ordinary Differential Equation Solver (soon)
  * Multidimensional curvefitting (soon)
  * Multidimensional minimization (soon)

* use Perl+Math::GSL as glue between sensors/data source and computer algebra system (like Matlab/Mathematica/Maple/Macsyma ... )
  * why isn't there a Perl CAS or something like sciPy.org ?

* why it is better than pure Perl
  * 2.5x faster numeric sort, sort_k_largest, sort_k_smallest functions

* why Math::GSL + Perl beats "whatever you're doing now"
  * throwaway analysis code is 80% data translation, 20% heavy-lifting
  * easier to work with sensor data, networking
  * somewhere between matlab and a monolithic fortran solver on a cluster of mainframes

[Podcast](http://podasp.com/episodes/P/PD/PDX.pm/2385/20080910__MathGSL_Scientific_Comp__2385.mp3) [Slides](http://leto.net/gitweb/?p=presentations.git;a=blob_plain;f=ScientificComputingWithPerlAndMathGSL/pres.pdf)
