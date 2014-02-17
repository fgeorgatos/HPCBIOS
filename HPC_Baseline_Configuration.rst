HPC Baseline Configuration
==========================

.. topic:: Introduction

  HPCBIOS is an effort to setup a common, well-documented and reproducible,
  environment spanning across multiple HPC systems & sites.

  HPC Baseline Configuration (BC) is an effort to define a common set of
  capabilities and functions so that users can work more productively and
  collaboratively when using the HPC resources at multiple computing
  sites within the HPCBIOS project context. This will be accomplished by
  defining and developing a common set of capabilities and functions so
  that users can focus energy on their research effort,
  as opposed to wrestling with site-specific policies and procedures.

  It is modeled after a similar effort taking place elsewhere among 6 HPC sites in the US and,
  in effect, it is an extension upon it (notably Compliance Matrix):

  `HPC-BC <http://centers.hpc.mil/consolidated/bc/>`_.

  The effort of this project keeps marching on helping users work more
  productively by updating existing policies to accommodate emerging needs,
  integrating new capabilities that must be consistent across the HPC
  enterprise, or just providing a sounding board for users experiencing
  difficulties with an HPC environment.

  * The keywords *MUST*, *MUST NOT*, *REQUIRED*, *SHALL*, *SHALL NOT*, *SHOULD*, *SHOULD NOT*,
    *RECOMMENDED*, *MAY*, and *OPTIONAL* are to be interpreted as described in :rfc:`2119`.

About the Baseline Configuration
--------------------------------

There is a growing community of HPCBIOS users who need to work on data
and computation-intensive problems spread across multiple computing
sites and services. Recent discussions show that over half of users
may need accounts at more than one site.

The main goal of the HPC Baseline Configuration activity is to define
and establish a common set of capabilities and functions so that users
can compute productively and collaboratively when using the HPC
resources at multiple computing sites.

Compliance Matrix
-----------------

.. |y| image:: images/check.png
.. |n| image:: images/error.png
.. |a| image:: images/thumbs_up.png
.. |d| image:: images/thumbs_down.png
.. |i| image:: images/information.png
.. |w| image:: images/warning.png

Use notation |y| |n| |a| |d| |i| |w| respectively standing for: *yes, no, agree, disagree, information notice, warning notice*.

+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| Policy tag #       | Policy Topics                                                            | Chaos   | Gaia   | G5K   |
+====================+==========================================================================+=========+========+=======+
| |HPCBIOS_05_01|    | Multiple-Version Software                                                | |y|     | |y|    |       |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| |HPCBIOS_05-05|    | Queue Names                                                              | |a|     | |a|    |       |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| |HPCBIOS_05-06|    | Login Shells                                                             | |y|     | |y|    | |y|   |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| |HPCBIOS_06-01|    | Open Source Math Libraries                                               | |y|     | |y|    |       |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| |HPCBIOS_06-04|    | Editors and Scripting Tools                                              | |y|     | |y|    | |y|   |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| |HPCBIOS_06-05|    | Baseline Set of Debuggers                                                | |y|     | |y|    |       |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| |HPCBIOS_06-15|    | Sample Code Repository                                                   | |a|     | |a|    |       |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| |HPCBIOS_06-17|    | Multiple-Version Software Access via Modules                             | |y|     | |y|    |       |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| |HPCBIOS_06-19|    | Open Source Utilities                                                    | |y|     | |y|    | |y|   |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| |HPCBIOS_07-02|    | Open Source Performance and Profiling Tools                              | |y|     | |y|    |       |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| |HPCBIOS_07-03|    | Common Set of Open Source Compilers                                      | |y|     | |y|    | |a|   |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| |HPCBIOS_10-01|    | New/Returning User Welcome Letter                                        | |a|     | |a|    | |a|   |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| |HPCBIOS_10-02|    | Common Open Source High Productivity Languages                           | |y|     | |y|    | |a|   |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| |HPCBIOS_2012-80|  | Common Set of DFT codes                                                  | |a|     | |a|    |       |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| |HPCBIOS_2012-90|  | Software Tools and Development Environment                               | |y|     | |y|    |       |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| |HPCBIOS_2012-91|  | Modules Namespace for HPC sites                                          | |y|     | |y|    |       |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| |HPCBIOS_2012-92|  | EasyBuild HPC Software Development Environment                           | |y|     | |y|    |       |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| |HPCBIOS_2012-93|  | Life Sciences Productivity Environment                                   | |y|     | |y|    |       |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| |HPCBIOS_2012-94|  | Bioinformatics and Computational Biology Productivity Environment        | |y|     | |y|    |       |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| |HPCBIOS_2012-95|  | Molecular Dynamics Productivity Environment                              | |a|     | |a|    |       |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| |HPCBIOS_2012-96|  | Common Set of Commercial Compilers                                       | |a|     | |y|    |       |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| |HPCBIOS_2012-97|  | Climate Science Productivity Environment                                 | |a|     | |a|    |       |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| |HPCBIOS_2012-98|  | Common Set of Environment Variables                                      | |a|     | |a|    |       |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| |HPCBIOS_2012-99|  | GPU Productivity Environment                                             | |n|     | |a|    | |n|   |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+
| |HPCBIOS_2013-01|  | Common Dependencies for Life Science Applications                        | |a|     | |a|    | |a|   |
+--------------------+--------------------------------------------------------------------------+---------+--------+-------+

.. note::
  Non-Compliance Disclaimer

  Site compliance assures that the minimum guidelines of the policy have
  been met by the Site.
  Sites may, at their discretion, exceed the minimum guidelines and
  still remain in compliance.
  Periodic checks may need be performed to ensure compliance is maintained.

  Note, there can be valid reasons for not being compliant with a policy.
  For example, non-compliance may be acceptable especially if it implies removal of
  an existing capability or function from a given system; also, for generic operational reasons
  or, if the HPC system affected is scheduled for decommissioning in the near future.

  **Non-compliance is not an issue, as long as the documentation above is consistent
  and the users are informed about status, promptly.**

This document was last rebuilt on: |today|.

.. |HPCBIOS_05_01| replace:: [:ref:`HPCBIOS_05-01 <HPCBIOS_05-01>`]
.. |HPCBIOS_05-05| replace:: [:ref:`HPCBIOS_05-05 <HPCBIOS_05-05>`]
.. |HPCBIOS_05-06| replace:: [:ref:`HPCBIOS_05-06 <HPCBIOS_05-06>`]
.. |HPCBIOS_06-01| replace:: [:ref:`HPCBIOS_06-01 <HPCBIOS_06-01>`]
.. |HPCBIOS_06-04| replace:: [:ref:`HPCBIOS_06-04 <HPCBIOS_06-04>`]
.. |HPCBIOS_06-05| replace:: [:ref:`HPCBIOS_06-05 <HPCBIOS_06-05>`]
.. |HPCBIOS_06-15| replace:: [:ref:`HPCBIOS_06-15 <HPCBIOS_06-15>`]
.. |HPCBIOS_06-17| replace:: [:ref:`HPCBIOS_06-17 <HPCBIOS_06-17>`]
.. |HPCBIOS_06-19| replace:: [:ref:`HPCBIOS_06-19 <HPCBIOS_06-19>`]
.. |HPCBIOS_07-02| replace:: [:ref:`HPCBIOS_07-02 <HPCBIOS_07-02>`]
.. |HPCBIOS_07-03| replace:: [:ref:`HPCBIOS_07-03 <HPCBIOS_07-03>`]
.. |HPCBIOS_10-01| replace:: [:ref:`HPCBIOS_10-01 <HPCBIOS_10-01>`]
.. |HPCBIOS_10-02| replace:: [:ref:`HPCBIOS_10-02 <HPCBIOS_10-02>`]
.. |HPCBIOS_2012-80| replace:: [:ref:`HPCBIOS_2012-80 <HPCBIOS_2012-80>`]
.. |HPCBIOS_2012-90| replace:: [:ref:`HPCBIOS_2012-90 <HPCBIOS_2012-90>`]
.. |HPCBIOS_2012-91| replace:: [:ref:`HPCBIOS_2012-91 <HPCBIOS_2012-91>`]
.. |HPCBIOS_2012-92| replace:: [:ref:`HPCBIOS_2012-92 <HPCBIOS_2012-92>`]
.. |HPCBIOS_2012-93| replace:: [:ref:`HPCBIOS_2012-93 <HPCBIOS_2012-93>`]
.. |HPCBIOS_2012-94| replace:: [:ref:`HPCBIOS_2012-94 <HPCBIOS_2012-94>`]
.. |HPCBIOS_2012-95| replace:: [:ref:`HPCBIOS_2012-95 <HPCBIOS_2012-95>`]
.. |HPCBIOS_2012-96| replace:: [:ref:`HPCBIOS_2012-96 <HPCBIOS_2012-96>`]
.. |HPCBIOS_2012-97| replace:: [:ref:`HPCBIOS_2012-97 <HPCBIOS_2012-97>`]
.. |HPCBIOS_2012-98| replace:: [:ref:`HPCBIOS_2012-98 <HPCBIOS_2012-98>`]
.. |HPCBIOS_2012-99| replace:: [:ref:`HPCBIOS_2012-99 <HPCBIOS_2012-99>`]
.. |HPCBIOS_2013-01| replace:: [:ref:`HPCBIOS_2013-01 <HPCBIOS_2013-01>`]
