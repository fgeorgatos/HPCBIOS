.. _HPCBIOS_2012-99:

HPCBIOS_2012-99: GPU Productivity Environment
=============================================

.. note::

  GPU productivity environments have recently become an important part of scientific computing and visualization. The following is an attempt to define which ones are relevant for HPCBIOS compliant sites and set an action plan.

  * BC Policy: HPCBIOS_2012-99
  * Date of Policy: 1st November 2012

The main objective of this policy is to provide the following common GPU
productivity environment across all HPCBIOS resources:

+---------------------------------------+------------------------+--------------------+--------------------------------------------------------------------------+
| Package/Tool                          | Requested version(s)   | Compliance level   | Reference                                                                |
+=======================================+========================+====================+==========================================================================+
| CUDA Toolkit                          | v4.0                   | MUST               | http://developer.nvidia.com/cuda-toolkit-40                              |
+---------------------------------------+------------------------+--------------------+--------------------------------------------------------------------------+
| pyCUDA                                | 2011.2.1               | MUST               | http://mathema.tician.de/software/pycuda                                 |
+---------------------------------------+------------------------+--------------------+--------------------------------------------------------------------------+
| pyOpenCL                              | 2011.2                 | MUST               | http://mathema.tician.de/software/pyopencl                               |
+---------------------------------------+------------------------+--------------------+--------------------------------------------------------------------------+
| MAGMA                                 | v1.1                   | MUST               | http://icl.cs.utk.edu/magma                                              |
+---------------------------------------+------------------------+--------------------+--------------------------------------------------------------------------+
| ViennaCL                              | 1.2.0                  | MUST               | http://viennacl.sourceforge.net                                          |
+---------------------------------------+------------------------+--------------------+--------------------------------------------------------------------------+
| AMD math library for OpenCL (APPML)   | v1.4                   | MUST               | http://developer.amd.com/libraries/appmathlibs/Pages/default.aspx        |
+---------------------------------------+------------------------+--------------------+--------------------------------------------------------------------------+
| Intel OpenCL SDK                      | v1.5                   | SHOULD             | http://software.intel.com/en-us/articles/vcsource-tools-opencl-sdk       |
+---------------------------------------+------------------------+--------------------+--------------------------------------------------------------------------+
| CULA                                  | r12                    | SHOULD             | http://www.culatools.com                                                 |
+---------------------------------------+------------------------+--------------------+--------------------------------------------------------------------------+
| gputools R package                    | v0.26                  | SHOULD             | http://cran.r-project.org/web/packages/gputools/index.html               |
+---------------------------------------+------------------------+--------------------+--------------------------------------------------------------------------+
| rCUDA                                 | v3.1                   | SHOULD             | http://www.rCUDA.net                                                     |
+---------------------------------------+------------------------+--------------------+--------------------------------------------------------------------------+

These GPU productivity environment will be supplemented with other such
productivity tools as they become available on allocated systems.
