.. _HPCBIOS_2012-99:

HPCBIOS_2012-99: GPU Productivity Environment
=============================================

.. note::

  GPU productivity environments have recently become an important part of scientific computing
  and visualization. The following is an attempt to define which ones are relevant for HPCBIOS
  compliant sites and set an action plan.

  * BC Policy: HPCBIOS_2012-99
  * Date of Policy: 2012-12-15

The main objective of this policy is to provide the following common GPU
productivity environment across all HPCBIOS resources:

+---------------------------------------+------------------------+--------------------+--------------------------------------------------------------------------+
| Package/Tool                          | Requested version(s)   | Compliance level   | Reference                                                                |
+=======================================+========================+====================+==========================================================================+
| **CUDA Toolkit**                      | **v4.2 or later**      | MUST               | http://developer.nvidia.com/cuda-toolkit-40                              |
+---------------------------------------+------------------------+--------------------+--------------------------------------------------------------------------+
| **PyCUDA**                            | 2012.1                 | MUST               | http://mathema.tician.de/software/pycuda                                 |
+---------------------------------------+------------------------+--------------------+--------------------------------------------------------------------------+
| PyOpenCL                              | 2012.1                 | MUST               | http://mathema.tician.de/software/pyopencl                               |
+---------------------------------------+------------------------+--------------------+--------------------------------------------------------------------------+
| MAGMA                                 | v1.3                   | MUST               | http://icl.cs.utk.edu/magma                                              |
+---------------------------------------+------------------------+--------------------+--------------------------------------------------------------------------+
| ViennaCL                              | v1.4.2                 | MUST               | http://viennacl.sourceforge.net                                          |
+---------------------------------------+------------------------+--------------------+--------------------------------------------------------------------------+
| AMD math library for OpenCL (APPML)   | v1.10                  | SHOULD             | http://developer.amd.com/libraries/appmathlibs/Pages/default.aspx        |
+---------------------------------------+------------------------+--------------------+--------------------------------------------------------------------------+
| **Rgputools** for R language          | v0.28                  | SHOULD             | http://cran.r-project.org/web/packages/gputools                          |
+---------------------------------------+------------------------+--------------------+--------------------------------------------------------------------------+
| Intel OpenCL SDK                      | v1.5                   | SHOULD             | http://software.intel.com/en-us/articles/vcsource-tools-opencl-sdk       |
+---------------------------------------+------------------------+--------------------+--------------------------------------------------------------------------+
| CULA & CULASPARSE                     | R16a & S4              | SHOULD             | http://www.culatools.com                                                 |
+---------------------------------------+------------------------+--------------------+--------------------------------------------------------------------------+
| rCUDA                                 | v4.0.1                 | SHOULD             | http://www.rCUDA.net                                                     |
+---------------------------------------+------------------------+--------------------+--------------------------------------------------------------------------+
| VCL                                   | v1.19                  | SHOULD             | http://www.mosix.org/txt_vcl.html                                        |
+---------------------------------------+------------------------+--------------------+--------------------------------------------------------------------------+

This GPU productivity environment will be supplemented with other such
productivity tools as they become available on allocated systems.

Potential sources of information for further future upgrades of this list include:
  * http://brainarray.mbni.med.umich.edu/brainarray/rgpgpu/
  * http://www.nvidia.com/object/gpu-test-drive.html
