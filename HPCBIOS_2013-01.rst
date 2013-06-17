.. _HPCBIOS_2013-01:

HPCBIOS_2013-01: Common Dependencies for Life Science Applications
==================================================================

.. note::
  As the number of Life Science applications increases, it becomes
  more and more pronounced the need to stabilize on a substrate
  of common dependencies; this permis to mix together software depending
  on multiple (dynamic) libraries, with predictable results and no conflicts.
  This need is particularly important when an HPC platform delivers
  Bioinformatics packages via modules, which need to be combined in a pipeline
  or simply loaded as one unit, for reproducibility purposes.

  * BC Policy: HPCBIOS_2013-01
  * Date of Policy: 2013-06-15

A list has been compiled with the most common dependencies for Life Science applications;
some room for (justified) deviations is provided by softening the compliance level to SHOULD:

+--------------+-----------------------+--------------------+
| Name         | Prefered version(s)   | Compliance level   |
+==============+=======================+====================+
| bzip2        | v1.0.6                | MUST               |
+--------------+-----------------------+--------------------+
| zlib         | v1.2.7                | MUST               |
+--------------+-----------------------+--------------------+
| libreadline  | v6.2                  | MUST               |
+--------------+-----------------------+--------------------+
| ncurses      | v5.9                  | MUST               |
+--------------+-----------------------+--------------------+
| Python       | v2.7.3                | SHOULD             |
+--------------+-----------------------+--------------------+
| Boost        | v1.51.0-Python-2.7.3  | SHOULD             |
+--------------+-----------------------+--------------------+
| SAMtools     | v0.1.18               | SHOULD             |
+--------------+-----------------------+--------------------+
| Perl         | v5.16.3               | SHOULD             |
+--------------+-----------------------+--------------------+
| Java         | v1.7.0_10             | SHOULD             |
+--------------+-----------------------+--------------------+
| libpng       | v1.5.13               | SHOULD             |
+--------------+-----------------------+--------------------+

N.B.
The *GNU-compatible suite MUST be implemented* for compliance with this policy on a given site.
*libreadline* SHOULD be built with *ncurses* as dependency.

Kindly notify -if this policy is inadequate for your work-
both your local site technical representative & HPCBIOS user-support.

