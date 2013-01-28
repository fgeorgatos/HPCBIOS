.. _HPCBIOS_2012-96:

HPCBIOS_2012-96: Common Set of Commercial Compilers
===================================================

.. note::

  Providing commercial compilers is imperative for many user groups.

  * BC Policy: HPCBIOS_2012-96
  * Date of Policy: 2012-12-15

Thus, to increase user productivity and expand commonality across
HPCBIOS sites, sites shall install the following commercial compilers,
either through a user’s default path or the availability of a module
file. In addition, in order to truly take advantage of the modern HPC
environment, *MPI support for the commercial compilers suite MUST be
implemented* for compliance with this policy.

+--------------------------+------------------------------+--------------------+--------------------------------------------------------------------+
| Name                     | Prefered version(s)          | Compliance level   | Comments                                                           |
+==========================+==============================+====================+====================================================================+
| Intel C/C++ Compiler     |      **v11, v12.1, v13.x**   | MUST               | icc/11.1.073 (v11), icc/2011.6.233 (v12.1), icc/2013.1.117 (v13.x) |
+--------------------------+------------------------------+--------------------+--------------------------------------------------------------------+
| Intel Fortran Compiler   | v10, **v11, v12.1, v13.x**   | MUST               | icc/11.1.073 (v11), icc/2011.6.233 (v12.1), icc/2013.1.117 (v13.x) |
+--------------------------+------------------------------+--------------------+--------------------------------------------------------------------+
| Lahey/Fujitsu Fortran    | v6.2 & v8.1                  | SHOULD             | This may be required by certain climate community members          |
+--------------------------+------------------------------+--------------------+--------------------------------------------------------------------+

It is at the discretion of each site which (if any) libraries will be
compiled with the commercial compilers. Ultimately, it will be the
responsibility of each user of the commercial compilers to create the
libraries that they require for their compiled software.

.. note::

  The current form of the policy currently does not specify 32 bit vs 64
  bit version, though it is expected that the native architecture of a
  given system (typically 64 bits) is supported as the default target,
  while the other is optional but desired to have (typically 32 bits).

