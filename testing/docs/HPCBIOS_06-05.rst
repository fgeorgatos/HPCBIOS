.. _HPCBIOS_06-05:

HPCBIOS_06-05: Baseline Set of Debuggers
========================================

.. note::
  This policy defines a baseline set of debuggers that can assist in HPC users for parallel codes.

  * BC Policy: HPCBIOS_06-05
  * Date of Policy: 2012-12-15

The lack of a baseline set of debuggers can compound what is arguably
one of the most difficult tasks in scientific code development -
debugging new algorithms. The process of tracking down bugs in large
scientific codes is frustrating and time consuming. Having to learn a
new tool to do so limits efficiency and productivity of valuable HPC programmers.

Somebody can argue that code should be written without bugs but, until that day
arrives there is a dire need for using debuggers and building expertise upon them.

For these reasons a baseline set of debuggers, preferred to be installed
at all systems, has been identified by examining what is in use at
different sites and what can be used across a variety of platforms.
At this time, these packages are included in the RECOMMENDED baseline set:

+---------------+------------------------------------------------------------------------------------+---------------------+----------------------------------------------------+
| Debugger Name | Description                                                                        | Compliance Level    | References                                         |
+===============+====================================================================================+=====================+====================================================+
| **GDB**       | A freeware debugger offered by the GNU project, covered by the GNU public license. | MUST                | http://www.gnu.org/software/gdb/gdb.html           |
+---------------+------------------------------------------------------------------------------------+---------------------+----------------------------------------------------+
| Eclipse PTP   | Parallel Tools Platform supports MPI, OpenMP & UPC; as well as OpenSHMEM & OpenACC | SHOULD              | http://www.eclipse.org/ptp/                        |
+---------------+------------------------------------------------------------------------------------+---------------------+----------------------------------------------------+
| Allinea DDT   | A popular suite for debugging in the HPC realm offered by Allinea.                 | SHOULD (commercial) | http://www.allinea.com/products/ddt/               |
+---------------+------------------------------------------------------------------------------------+---------------------+----------------------------------------------------+
| Totalview     | A long standing de-facto standard for debugging in the HPC realm offered           | SHOULD (commercial) | http://www.roguewave.com/products/totalview.aspx   |
|               | by  TotalView Technologies                                                         |                     |                                                    |
+---------------+------------------------------------------------------------------------------------+---------------------+----------------------------------------------------+
| MemoryScape   | Dynamic memory debugging for monitoring heap allocations, memory leaks             | MAY (commercial)    | http://www.roguewave.com/products/memoryscape.aspx |
|               | memory overruns, and memory usage; by Rogue Wave software                          |                     |                                                    |
+---------------+------------------------------------------------------------------------------------+---------------------+----------------------------------------------------+

In order to be compliant, a center must have at least the "MUST" class of these
debuggers installed and in the standard login path across all nodes or,
available via modules mechanism.

In addition, the GUI interface for TotalView/DDT, when available, must be
operational and accessible from the compute nodes of the allocated system.

Potential sources of information for further future upgrades of this list include:
  * http://wiki.scinethpc.ca/wiki/images/c/ce/Best-practice-debug.pdf
  * http://www.nersc.gov/users/software/debugging-and-profiling/
  * http://sebastien.dinot.free.fr/liens_dev_c_cpp.html
  * http://user.cscs.ch/fileadmin/user_upload/customers/CSCS_Application_Data/Files/Presentations/Courses_Ws_2011/Multi-Threaded_Course_Feb11/debug.pdf
  * http://www.scalalife.eu/book/export/html/115 
  * http://www.acrc.a-star.edu.sg/10/code_development.html

Kindly notify -if this policy is inadequate for your work-
both your local site technical representative & HPCBIOS user-support.

