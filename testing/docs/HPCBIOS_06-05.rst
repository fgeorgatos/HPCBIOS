.. _HPCBIOS_06-05:

HPCBIOS_06-05: Baseline Set of Debuggers
========================================

.. note::
 A user may specify any login shell in the login shell baseline as the default shell on a new user application.

  * BC Policy: HPCBIOS_06-05
  * Date of Policy: 1st November 2012

The lack of a baseline set of debuggers can compound what is arguably
one of the most difficult tasks in scientific code development —
debugging new algorithms. The process of tracking down bugs in large
scientific codes is frustrating and time consuming. Having to learn a
new tool to do so limits efficiency and productivity of valuable HPC
programmers.

For these reasons, a baseline set of debuggers preferred to be installed
at all centers has been identified by examining what is in use at
different centers and what can be used across a variety of platforms. At
this time, only three packages are included in the baseline set:

+-----------------+------------------------------------------------------------------------------------------------------+-----------------------+----------------------------------------------+
| Debugger Name   | Description                                                                                          | Compliance Level      | References                                   |
+=================+======================================================================================================+=======================+==============================================+
| **GDB**         | A freeware debugger offered by the GNU project, covered by the GNU public license.                   | MUST                  | http://www.gnu.org/software/gdb/gdb.html   |
+-----------------+------------------------------------------------------------------------------------------------------+-----------------------+----------------------------------------------+
| Allinea DDT     | A popular suite for debugging in the HPC realm offered by Allinea.                                   | SHOULD (commercial)   | http://allinea.com/ddt                     |
+-----------------+------------------------------------------------------------------------------------------------------+-----------------------+----------------------------------------------+
| Totalview       | A long standing de-facto standard for debugging in the HPC realm offered by TotalView Technologies   | SHOULD (commercial)   | http://www.totalviewtech.com/              |
+-----------------+------------------------------------------------------------------------------------------------------+-----------------------+----------------------------------------------+

In order to be compliant, a center must have at least the first of these
debuggers installed and in the standard login path across all nodes. In
addition, the GUI interface for TotalView, when available, must be
operational and accessible from the compute nodes of any allocated system.
