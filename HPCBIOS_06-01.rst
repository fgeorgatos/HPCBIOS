.. _HPCBIOS_06-01:

HPCBIOS_06-01: Common Set of Open Source Math Libraries
=======================================================

.. note::
  This policy defines a set of open source math libraries and their
  consistent maintenance (same version and same configuration) across the
  resources at the participating sites. Having same configuration is dependent
  on system compatibility, and also, some libraries may have slightly
  different configurations due to architectural differences.
  These differences, however, will not affect the use of the libraries.
  A user moving from one resource to another will notice no difference between
  the installations and it is expected to find an optimized version of that library.

  * BC Project: HPCBIOS_06-01
  * Date of Policy: 2012-12-15

The suite of maintained packages consists of:

+---------------+------------------------------------------------------------------------------------------+--------------------+-----------------------------------------------+
| Library API   | Purpose                                                                                  | Compliance level   | References                                    |
+===============+==========================================================================================+====================+===============================================+
| **FFTW**      | Library for computing Discrete Fourier Transforms                                        | MUST               | http://www.fftw.org/                          |
|               | Both MPI and non-MPI versions should be provided.                                        |                    |                                               |
+---------------+------------------------------------------------------------------------------------------+--------------------+-----------------------------------------------+
| **PETSc**     | Suite of scientific computing routines                                                   | MUST               | http://www.mcs.anl.gov/petsc/                 |
+---------------+------------------------------------------------------------------------------------------+--------------------+-----------------------------------------------+
| **LAPACK**    | Software library of numerical linear algebra routines                                    | MUST               | http://www.netlib.org/lapack/                 |
+---------------+------------------------------------------------------------------------------------------+--------------------+-----------------------------------------------+
| **ScaLAPACK** | Subset of parallelized LAPACK routines                                                   | MUST               | http://www.netlib.org/scalapack/              |
+---------------+------------------------------------------------------------------------------------------+--------------------+-----------------------------------------------+
| **BLAS**      | Basic linear algebra routines; this could be any of:                                     | MUST               | http://www.netlib.org/blas/                   |
|               |   * **ATLAS**                                                                            |                    | http://math-atlas.sourceforge.net/            |
|               |   * **MKL**                                                                              |                    | http://software.intel.com/en-us/intel-mkl     |
|               |   * **OpenBLAS** or GotoBLAS                                                             |                    | http://www.tacc.utexas.edu/tacc-projects/#blas|
|               |                                                                                          |                    | https://github.com/xianyi/OpenBLAS            |
+---------------+------------------------------------------------------------------------------------------+--------------------+-----------------------------------------------+
| **GSL**       | C/C+ library with a wide variety of mathematical routines                                | MUST               | http://www.gnu.org/s/gsl/                     |
+---------------+------------------------------------------------------------------------------------------+--------------------+-----------------------------------------------+
| ARPACK        | Solution of Eigenvalues/Eigenvectors                                                     | MUST               | http://www.caam.rice.edu/software/ARPACK/     |
+---------------+------------------------------------------------------------------------------------------+--------------------+-----------------------------------------------+
| SuperLU       | Direct solution of sparse linear systems of equations                                    | SHOULD             | http://crd.lbl.gov/~xiaoye/SuperLU            |
+---------------+------------------------------------------------------------------------------------------+--------------------+-----------------------------------------------+
| **SPRNG**     | Pseudo-Random Number Generators for Stochastic computation via Monte Carlo methods et al | SHOULD             | http://sprng.cs.fsu.edu/                      |
+---------------+------------------------------------------------------------------------------------------+--------------------+-----------------------------------------------+

Change notification
-------------------

Guidelines:

- This policy MUST provide the default implementation for LINPACK/BLAS functions
- Notification MUST be sent to the system's helpdesk announcing the new version and describing how to access it and use it
- The helpdesk MUST be given a minimum of 2 weeks notice when the new version becomes the default version
- It is the responsibility of the individual sites to notify their users of any changes

.. seealso::
  Native Libraries

  As regards packages ScaLAPACK, LAPACK and/or ATLAS, they MAY not be installed
  whenever a system includes native libraries such as PESSL (Parallel
  ESSL) ACML or, MKL (Math kernel Libraries) that fully provide the same
  functionality and interface. However, if an explicit request is made to
  have open source ScaLAPACK, LAPACK and/or ATLAS available on a system,
  then these packages MUST also be installed.

Support

The helpdesk team (User Support) maintains the suite of software listed
in this policy, and it also provides the needed support channels.
