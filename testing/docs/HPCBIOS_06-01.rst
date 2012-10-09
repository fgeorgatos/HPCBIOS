HPCBIOS_06-01: Common Set of Open Source Math Libraries
=======================================================

.. note::
  This policy defines a set of open source math libraries and their
  consistent maintenance (same version and same configuration) across the
  resources at the participating centers. Same configuration is dependent
  on system compatibility, and also, some libraries may have slightly
  different configurations due to architectural differences. These
  differences, however, will not affect the use of the libraries. A user
  moving from one resource to another will notice no difference between
  the installations and it is expected to find an optimized version of
  that library.

  * BC Project: HPCBIOS_06-01
  * Date of Policy: 1st November 2012

The suite of maintained packages consists of:

+---------------+----------------------------------------------------------------------------------------------------+--------------------+-----------------------------------------------+
| Library API   | Purpose                                                                                            | Compliance level   | References                                    |
+===============+====================================================================================================+====================+===============================================+
| ARPACK        | Solution of Eigenvalues/Eigenvectors                                                               | SHOULD             | [http://www.caam.rice.edu/software/ARPACK/]   |
+---------------+----------------------------------------------------------------------------------------------------+--------------------+-----------------------------------------------+
| FFTW          | Library for computing Discrete Fourier Transforms ; Both MPI and non-MPI versions are maintained   | MUST               | [http://www.fftw.org/]                        |
+---------------+----------------------------------------------------------------------------------------------------+--------------------+-----------------------------------------------+
| PETSc         | Suite of scientific computing routines                                                             | MUST               | [http://www.mcs.anl.gov/petsc/]               |
+---------------+----------------------------------------------------------------------------------------------------+--------------------+-----------------------------------------------+
| SuperLU       | Direct solution of sparse linear systems of equations                                              | SHOULD             | [http://crd.lbl.gov/~xiaoye/SuperLU]          |
+---------------+----------------------------------------------------------------------------------------------------+--------------------+-----------------------------------------------+
| LAPACK        | Software library of numerical linear algebra routines                                              | MUST               | [http://www.netlib.org/lapack/]               |
+---------------+----------------------------------------------------------------------------------------------------+--------------------+-----------------------------------------------+
| ScaLAPACK     | Subset of parallelized LAPACK routines                                                             | MUST               | [http://www.netlib.org/scalapack/]            |
+---------------+----------------------------------------------------------------------------------------------------+--------------------+-----------------------------------------------+
| BLAS          | Basic linear algebra routines * ATLAS * GotoBLAS                                                   | MUST               | [http://www.netlib.org/blas/]                 |
+---------------+----------------------------------------------------------------------------------------------------+--------------------+-----------------------------------------------+
| GSL           | C/C+ library with a wide variety of mathematical routines                                          | MUST               | [http://www.gnu.org/s/gsl/]                   |
+---------------+----------------------------------------------------------------------------------------------------+--------------------+-----------------------------------------------+
| SPRNG         | Pseudo-Random Number Generators for Stochastic computation via Monte Carlo methods et al           | SHOULD             | [http://sprng.cs.fsu.edu/]                    |
+---------------+----------------------------------------------------------------------------------------------------+--------------------+-----------------------------------------------+

Change notification
===================

New versions of supported libraries will initially be installed as
non-default. Notification will be sent to the project helpdesk
announcing the new version and describing how to access it and use it.
The helpdesk will be given a minimum of 2 weeks notice when the new
version becomes the default version. The old version will not be
deleted, but notice will be sent to the helpdesk describing how users
can continue to use the old version. It is the responsibility of the
individual centers to notify their users of any changes. This change
notification is in the absence of any baseline configuration change
notification policy that may exist. Any baseline configuration policy on
change notification supersedes the change notification listed in this
policy. The minimum of versions that will be kept, MUST follow BC
[HPCBIOS_05-01|HPCBIOS_05-01] policy. Old versions MAY be deleted when there
are three newer versions available.

.. seealso::
  Native Libraries

  The packages ScaLAPACK, LAPACK and/or ATLAS will not be installed
  whenever a system includes native libraries such as PESSL (Parallel
  ESSL) ACML or, MKL (Math kernel Libraries) that fully provide the same
  functionality and interface. However, if an explicit request is made to
  have ScaLAPACK, LAPACK and/or ATLAS available on a system, then these
  packages will also be installed.

Support

The helpdesk team (User Support) maintains the suite of software listed
in this policy, and it also provides the needed support channels.

.. _`http://www.caam.rice.edu/software/ARPACK/`: http://www.caam.rice.edu/software/ARPACK/
.. _`http://www.fftw.org/`: http://www.fftw.org/
.. _`http://www.mcs.anl.gov/petsc/`: http://www.mcs.anl.gov/petsc/
.. _`http://crd.lbl.gov/~xiaoye/SuperLU`: http://crd.lbl.gov/~xiaoye/SuperLU
.. _`http://www.netlib.org/lapack/`: http://www.netlib.org/lapack/
.. _`http://www.netlib.org/scalapack/`: http://www.netlib.org/scalapack/
.. _`http://www.netlib.org/blas/`: http://www.netlib.org/blas/
.. _`http://sprng.cs.fsu.edu/`: http://sprng.cs.fsu.edu/
.. _`http://www.gnu.org/s/gsl/`: http://www.gnu.org/s/gsl/
