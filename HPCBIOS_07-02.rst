.. _HPCBIOS_07-02:

HPCBIOS_07-02: Common Open Source Performance and Profiling Tools
=================================================================

.. note::
  Performance and profiling tools are used on HPC sites for keeping codes execution times tamed.

  This policy defines a set of performance and profiling tools and promotes their
  consistent maintenance (ie maintain compatible versions and configuration)
  across all systems of compatible sites. Same configuration is dependent on
  system compatibility, and also, some libraries may have slightly
  different configurations due to architectural differences.
  These differences, however, SHALL NOT affect the use of the libraries.
  A user moving from one resource to another is not expected to notice significant difference between the installations.

  * BC Policy: HPCBIOS_07-02
  * Date of Policy: 2012-12-15

The suite of maintained packages consists of:

+------------------------+--------------------------------------------------------+--------------------+-------------------------------------------------------------------------+
| Tool                   | Description                                            | Compliance level   | Reference                                                               |
+========================+========================================================+====================+=========================================================================+
| **gprof**              | The GNU Profiler                                       | **MUST**           | http://www.gnu.org/software/binutils/                                   |
+------------------------+--------------------------------------------------------+--------------------+-------------------------------------------------------------------------+
| **PAPI**               | Consistent interface to hardware counters and events   | **MUST**           | http://icl.cs.utk.edu/papi                                              |
+------------------------+--------------------------------------------------------+--------------------+-------------------------------------------------------------------------+
| **Valgrind**           | Memory management analysis and profiling               | **MUST**           | http://valgrind.org/                                                    |
+------------------------+--------------------------------------------------------+--------------------+-------------------------------------------------------------------------+
|**Intel Vtune Analyzer**| performance optimization tool                          | SHOULD             | http://software.intel.com/en-us/articles/intel-vtune-amplifier-xe/      |
|                        | NOTE: not open source but still relevant               | (commercial)       |                                                                         |
+------------------------+--------------------------------------------------------+--------------------+-------------------------------------------------------------------------+
| UNITE                  | UNiform Integrated Tool Environment                    | SHOULD             | http://apps.fz-juelich.de/unite                                         |
+------------------------+--------------------------------------------------------+--------------------+-------------------------------------------------------------------------+

UNITE
~~~~~

The goal of UNITE is to provide a robust, portable, and integrated
environment for the debugging and performance analysis of parallel MPI,
OpenMP and hybrid MPI/OpenMP programs on high-performance compute
clusters. It consists of a set of well-accepted portable, mostly
open-source tools. UNITE itself includes:

  +--------------+-------------------------------------------------+---------------------------------------------+
  |  mpiP        | Lightweight, Scalable MPI Profiling             | http://mpip.sourceforge.net/                |
  +--------------+-------------------------------------------------+---------------------------------------------+
  | **SCALASCA** | Scalable trace analysis package                 | http://www.scalasca.org/                    |
  +--------------+-------------------------------------------------+---------------------------------------------+
  | **Vampir**   | Performance Optimization                        | http://www.vampir.eu/                       |
  +--------------+-------------------------------------------------+---------------------------------------------+
  |  TAU         | Performance analysis of parallel applications   | http://www.cs.uoregon.edu/Research/tau      |
  |              |   * Support for **PAPI** and **SCALASCA**       |                                             |
  |              |   * **PDT**: Source-level auto-instrumentation  |                                             |
  +--------------+-------------------------------------------------+---------------------------------------------+
  |  PerfSuite   | software performance analysis                   | http://perfsuite.ncsa.illinois.edu/         |
  +--------------+-------------------------------------------------+---------------------------------------------+
  |  other       | hpctoolkit periscope marmot **itac**            |                                             |
  |              | Extrae Paraver kcachegrind                      |                                             |
  +--------------+-------------------------------------------------+---------------------------------------------+

The packages will be installed and maintained as part of a consistent computational environment.

Potential sources of information for further future upgrades of this list include:
  * http://apps.fz-juelich.de/unite
  * http://www.vi-hps.org/tools/

Kindly notify -if this policy is inadequate for your work-
both your local site technical representative & HPCBIOS maintainers.

