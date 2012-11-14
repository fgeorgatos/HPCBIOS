.. _HPCBIOS_2011-92:

HPCBIOS_2011-92: EasyBuild Development Environment
==================================================

.. note::

  EasyBuild Development environment allows to build and use scientific computing software
  in a consistent and reproducible way: It can manage Software and Modules together.

  * BC Policy: HPCBIOS_2011-92
  * Date of Policy: 1st December 2012

The main objective of this policy is to provide EasyBuild, for a consistent software tree and module namespace across any HPCBIOS resources.

Scope
-----

EasyBuild_ is a tool developed over the course of last years and released for production use during 2012.

To be compliant with this policy, an HPC site MUST provide at least one production version of EasyBuild.
This can be done either in the default $PATH or, available via modules (as per ``module load easybuild``).
The default provided version MAY be customized as per local needs and SHOULD be working out of the box, as developers describe.

Example
-------


.. code-block:: sh

  $ sw@gaia-1:~$ module avail
  
  ------------- /opt/apps/testing/fgeorgatos/easybuild//modules/all --------------
  AMOS/3.1.0-goalf-1.1.0-no-OFED
  ASE/3.6.0.2515-goalf-1.1.0-no-OFED-Python-2.7.3
  ATLAS/3.8.4-gompi-1.1.0-no-OFED-LAPACK-3.4.0
  Armadillo/2.4.4-goalf-1.1.0-no-OFED-Python-2.7.3
  BLACS/1.1-gompi-1.1.0-no-OFED
  BWA/0.6.2-goalf-1.1.0-no-OFED
  Boost/1.49.0-goalf-1.1.0-no-OFED-Python-2.7.3
  Bowtie2/2.0.0-beta7-goalf-1.1.0-no-OFED
  CGAL/4.0-goalf-1.1.0-no-OFED-Python-2.7.3
  CMake/2.8.4-goalf-1.1.0-no-OFED
  CVXOPT/1.1.5-goalf-1.1.0-no-OFED-Python-2.7.3
  ClustalW2/2.1-goalf-1.1.0-no-OFED
  Cython/0.16-goalf-1.1.0-no-OFED-Python-2.7.3
  Docutils/0.9.1-goalf-1.1.0-no-OFED-Python-2.7.3
  Eigen/3.1.1-goalf-1.1.0-no-OFED
  FFC/1.0.0-goalf-1.1.0-no-OFED-Python-2.7.3
  FFTW/3.3.1-gompi-1.1.0-no-OFED
  FIAT/1.0.0-goalf-1.1.0-no-OFED-Python-2.7.3
  FSL/4.1.9-goalf-1.1.0-no-OFED
  GCC/4.6.3
  GMP/5.0.5-goalf-1.1.0-no-OFED
  GPAW/0.9.0.8965-goalf-1.1.0-no-OFED-Python-2.7.3
  GSL/1.15-goalf-1.1.0-no-OFED
  HDF5/1.8.7-goalf-1.1.0-no-OFED
  HDF5/1.8.7-goalf-1.1.0-no-OFED-parallel
  HDF5/1.8.9-goalf-1.1.0-no-OFED
  HPL/2.0-goalf-1.1.0-no-OFED
  Harminv/1.3.1-goalf-1.1.0-no-OFED
  Hypre/2.8.0b-goalf-1.1.0-no-OFED
  Infernal/1.1rc1-goalf-1.1.0-no-OFED
  Instant/1.0.0-goalf-1.1.0-no-OFED-Python-2.7.3
  JasPer/1.900.1-goalf-1.1.0-no-OFED
  Jinja2/2.6-goalf-1.1.0-no-OFED-Python-2.7.3
  LAPACK/3.4.0-gompi-1.1.0-no-OFED
  Libint/1.1.4-goalf-1.1.0-no-OFED
  METIS/4.0.1-goalf-1.1.0-no-OFED
  METIS/5.0.2-goalf-1.1.0-no-OFED
  MPFR/3.1.0-goalf-1.1.0-no-OFED
  MTL4/4.0.8878
  MUMmer/3.23-goalf-1.1.0-no-OFED
  Mercurial/2.3.2-goalf-1.1.0-no-OFED-Python-2.7.3
  MetaVelvet/1.2.01-goalf-1.1.0-no-OFED
  MrBayes/3.1.2-goalf-1.1.0-no-OFED
  OpenMPI/1.4.5-GCC-4.6.3-no-OFED
  PAPI/5.0.1-goalf-1.1.0-no-OFED
  PCRE/8.12-goalf-1.1.0-no-OFED
  PETSc/3.3-p2-goalf-1.1.0-no-OFED-Python-2.7.3
  ParMETIS/3.1.1-goalf-1.1.0-no-OFED
  ParMETIS/4.0.2-goalf-1.1.0-no-OFED
  Primer3/2.3.0-goalf-1.1.0-no-OFED
  Python/2.7.3-goalf-1.1.0-no-OFED
  RNAz/2.1-goalf-1.1.0-no-OFED
  SAMtools/0.1.18-goalf-1.1.0-no-OFED
  SCOTCH/5.1.12b_esmumps-goalf-1.1.0-no-OFED
  SHRiMP/2.2.3-goalf-1.1.0-no-OFED
  SOAPdenovo/1.05-goalf-1.1.0-no-OFED
  SWIG/2.0.4-goalf-1.1.0-no-OFED-Python-2.7.3
  ScaLAPACK/1.8.0-gompi-1.1.0-no-OFED-ATLAS-3.8.4-LAPACK-3.4.0-BLACS-1.1
  ScientificPython/2.8-goalf-1.1.0-no-OFED-Python-2.7.3
  Sphinx/1.1.3-goalf-1.1.0-no-OFED-Python-2.7.3
  SuiteSparse/3.7.0-goalf-1.1.0-no-OFED-withparmetis
  Szip/2.1-goalf-1.1.0-no-OFED
  Theano/0.5.0-goalf-1.1.0-no-OFED-Python-2.7.3
  Trilinos/10.12.2-goalf-1.1.0-no-OFED-Python-2.7.3
  UFC/2.0.5-goalf-1.1.0-no-OFED-Python-2.7.3
  UFL/1.0.0-goalf-1.1.0-no-OFED-Python-2.7.3
  Velvet/1.2.07-goalf-1.1.0-no-OFED
  ViennaRNA/2.0.7-goalf-1.1.0-no-OFED
  Viper/1.0.0-goalf-1.1.0-no-OFED-Python-2.7.3
  WRF/3.3.1-goalf-1.1.0-no-OFED-dmpar
  byacc/20120526-goalf-1.1.0-no-OFED
  bzip2/1.0.6-goalf-1.1.0-no-OFED
  expat/2.1.0-goalf-1.1.0-no-OFED
  flex/2.5.35-goalf-1.1.0-no-OFED
  freetype/2.4.10-goalf-1.1.0-no-OFED
  g2lib/1.2.4-goalf-1.1.0-no-OFED
  git/1.7.12-goalf-1.1.0-no-OFED
  glproto/1.4.16-goalf-1.1.0-no-OFED
  goalf/1.1.0-no-OFED
  gompi/1.1.0-no-OFED
  libffi/3.0.11-goalf-1.1.0-no-OFED
  libpng/1.5.10-goalf-1.1.0-no-OFED
  libpng/1.5.13-goalf-1.1.0-no-OFED
  libreadline/6.2-goalf-1.1.0-no-OFED
  libtool/2.4.2-goalf-1.1.0-no-OFED
  libunistring/0.9.3-goalf-1.1.0-no-OFED
  libxcb/1.8-goalf-1.1.0-no-OFED-Python-2.7.3
  libxml2/2.8.0-goalf-1.1.0-no-OFED
  libxml2/2.8.0-goalf-1.1.0-no-OFED-Python-2.7.3
  makedepend/1.0.4-goalf-1.1.0-no-OFED
  ncurses/5.9-goalf-1.1.0-no-OFED
  netCDF/4.1.3-goalf-1.1.0-no-OFED
  petsc4py/3.3-goalf-1.1.0-no-OFED-Python-2.7.3
  pkg-config/0.27.1-goalf-1.1.0-no-OFED
  setuptools/0.6c11-goalf-1.1.0-no-OFED-Python-2.7.3
  xcb-proto/1.7-goalf-1.1.0-no-OFED-Python-2.7.3
  xproto/7.0.23-goalf-1.1.0-no-OFED
  zlib/1.2.5-goalf-1.1.0-no-OFED
  zlib/1.2.7-goalf-1.1.0-no-OFED

References
----------

.. _EasyBuild  http://hpcugent.github.com/easybuild/

Kindly notify -if this policy is inadequate for your work-
both your local site technical representative & HPCBIOS user-support.
