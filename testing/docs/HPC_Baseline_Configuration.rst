HPC Baseline Configuration
==========================

.. note::
  HPC-BC is an effort to setup a common well-documented environment
  across multiple HPC sites.

  HPC Baseline Configuration (BC) is an effort to define a common set of
  capabilities and functions so that users can work more productively and
  collaboratively when using the HPC resources at multiple computing
  centers within the HPCBIOS project context. This will be accomplished by
  defining and developing a common set of capabilities and functions so
  that users can focus energy on their research as opposed to wrestling
  with center-specific policies and procedures.

  It is modeled after a similar effort taking place elsewhere among 6 HPC
  sites and in effect it is an extension upon it: `HPC-BC <http://www.ccac.hpc.mil/consolidated/bc>`_
  The effort of that BC team keeps marching on helping users work more
  productivity by updating existing policies to accommodate new users,
  integrating new capabilities that must be consistent across the
  enterprise, or just providing a sounding board for users experiencing
  difficulties with an HPC environment.

  * Keywords like MUST, MAY, SHOULD, RECOMMENDED are used in accordance
  with `RFC2119 <http://www.ietf.org/rfc/rfc2119.txt>`_

About the Baseline Configuration
--------------------------------

There is a growing community of HPCBIOS users who need to work on data
and computation-intensive problems spread across multiple computing
centers and services. Recent discussions show that over half of users
may need accounts at more than one center.

The main goal of the HPC Baseline Configuration activity is to define
and establish a common set of capabilities and functions so that users
can compute productively and collaboratively when using the HPC
resources at multiple computing centers.

Compliance Matrix
-----------------

.. |k| image:: images: check.gif
.. |x| image:: images: error.gif
.. |y| image:: images: thumbs_up.gif
.. |n| image:: images: thumbs_down.gif
.. |i| image:: images: information.gif
.. |w| image:: images: warning.gif

Use notation |k| |x| |y| |n| |i| |w| respectively standing for: yes, no, agree, disagree, information notice, attention notice.

+--------------------+--------------------------------------------------+---------+--------+-------+
| Policy tag #       | Policy Topics                                    | Chaos   | Gaia   | G5K   |
+--------------------+--------------------------------------------------+---------+--------+-------+
| [HPCBIOS\_05-01]   | Multiple-Version Software                        | (/)     | (/)    | (y)   |
+--------------------+--------------------------------------------------+---------+--------+-------+
| [HPCBIOS\_05-05]   | Queue Names                                      | (/)     | (/)    |       |
+--------------------+--------------------------------------------------+---------+--------+-------+
| [HPCBIOS\_05-06]   | Login Shells                                     | (/)     | (/)    | (y)   |
+--------------------+--------------------------------------------------+---------+--------+-------+
| [HPCBIOS\_06-01]   | Open Source Math Libraries                       | (/)     | (y)    | (y)   |
+--------------------+--------------------------------------------------+---------+--------+-------+
| [HPCBIOS\_06-04]   | Editors and Scripting Tools                      | (/)     | (/)    | (y)   |
+--------------------+--------------------------------------------------+---------+--------+-------+
| [HPCBIOS\_06-05]   | Set of Debuggers                                 | (/)     | (/)    |       |
+--------------------+--------------------------------------------------+---------+--------+-------+
| [HPCBIOS\_06-15]   | Sample Code Repository                           | (/)     | (/)    | (y)   |
+--------------------+--------------------------------------------------+---------+--------+-------+
| [HPCBIOS\_06-17]   | Multiple-Version Software Access via Modules     | (/)     | (/)    | (y)   |
+--------------------+--------------------------------------------------+---------+--------+-------+
| [HPCBIOS\_06-19]   | Open Source Utilities                            | (/)     | (/)    | (y)   |
+--------------------+--------------------------------------------------+---------+--------+-------+
| [HPCBIOS\_07-02]   | Open Source Performance and Profiling Tools      | (/)     | (/)    | (y)   |
+--------------------+--------------------------------------------------+---------+--------+-------+
| [HPCBIOS\_07-03]   | Common Set of Open Source Compilers              | (/)     | (/)    | (y)   |
+--------------------+--------------------------------------------------+---------+--------+-------+
| [HPCBIOS\_10-01]   | New/Returning User Welcome Letter                | (/)     | (/)    | (y)   |
+--------------------+--------------------------------------------------+---------+--------+-------+
| [HPCBIOS\_10-02]   | Common Open Source High Productivity Languages   | (y)     | (y)    | (y)   |
+--------------------+--------------------------------------------------+---------+--------+-------+
| [HPCBIOS\_11-99]   | GPU Productivity Environment                     | N/A     | (y)    | N/A   |
+--------------------+--------------------------------------------------+---------+--------+-------+
| [HPCBIOS\_11-98]   | Common Set of Environment Variables              | (/)     | (/)    |       |
+--------------------+--------------------------------------------------+---------+--------+-------+
| [HPCBIOS\_11-97]   | Climate Science Productivity Environment         |         | (y)    |       |
+--------------------+--------------------------------------------------+---------+--------+-------+
| [HPCBIOS\_11-96]   | Common Set of Commercial Compilers               | (/)     | (/)    |       |
+--------------------+--------------------------------------------------+---------+--------+-------+
| [HPCBIOS\_11-95]   | Molecular Dynamics Productivity Environment      |         | (y)    |       |
+--------------------+--------------------------------------------------+---------+--------+-------+

.. note::
  Non-Compliance Disclaimer

  Site compliance assures that the minimum guidelines of the policy have
  been met by the Center.
  Centers may, at their discretion, exceed the minimum guidelines and
  still remain in compliance.
  Periodic checks will be performed to ensure compliance is maintained.

  Note, there may be valid reasons for not being compliant with a policy.
  For example, non-compliance may be acceptable if it prevents removal of
  an existing capability or function from the Center’s systems or if the
  HPC system affected is scheduled for decommissioning in the near future.

  **Non-compliance is fine, as long as the documentation above is correct
  and the users are informed.**

