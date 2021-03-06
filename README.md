psi4numpy
=============

#####Author: Daniel G. A. Smith
#####Contact: dsmith@auburn.edu

The overall goal of psi4numpy is to provide clear, readable code for both learning
and development. Python is used to "plug" together low level languages and
provide an interface that is both simple to use and remains relatively fast
to execute. In this case Psi4 is used for molecular properties and integrals,
numpy/scipy is used for tensor operations and linear algebra.

The input files should be run as a normal psi4 input script; however,
it should be noted the output is printed to the command line instead of merged
with the psi4 output.

If you have comments, questions, or would like to contribute to the project please
feel free to email [me](mailto:dsmith@auburn.edu).

Most algorithms were taken directly from Daniel Crawford's programming [website](http://sirius.chem.vt.edu/wiki/doku.php?id=crawdad:programming).

A tutorial that covers the basics of numpy can be found [here](http://wiki.scipy.org/Tentative_NumPy_Tutorial).

#####Requirements:
- [Psi4](psicode.org)
- [Python](python.org) 2.7+
 - [Numpy](scipy.org) 1.7.2+
 - [Scipy](numpy.scipy.org) 0.13.0+

Conventions that, if possible, should be followed:
- All 2D numpy arrays will use the matrix class so the * operator is overloaded
  to perform matrix matrix multiplication.
  http://docs.scipy.org/doc/numpy/reference/generated/numpy.matrix.html

- All other operations will use einsum for clarity.
  http://docs.scipy.org/doc/numpy/reference/generated/numpy.einsum.html

- Tensordot should be avoided unless absolutely required.
  http://docs.scipy.org/doc/numpy/reference/generated/numpy.tensordot.html

