.. _HPCBIOS_2015-01:

HPCBIOS_2015-01: Biocompressors, for NGS data and bioinformatics
================================================================

.. note::

  As the volume of NGS data increases,
  it becomes more and more pronounced the need to optimally store and handle
  data coming from Next Generation Sequencing pipelines, in efficient manner.
  This is particularly true when such data reside in a common shared storage back-end
  which sustains big I/O pressure from hundreds or thousands of concurrent accesses.

  Maintaining the volume of data in compressed format, may achieve the following objectives:

  * Reduces considerably the required storage space (possibly as much as 5 or 6 times)
  * Provides an incentive for users, to perform correct stage-in/stage-out operations
  * May increase the speed with which I/O operations take place, if slow disk operations are minimized
  * Saturation of I/O subsystems may become less pronounced, or be postponed towards heavier loads

  The aim of this policy is to ensure that a sufficiently rich palette of entropy-conscious tools
  are available on machines which may be flooded by NGS data.

  * BC Policy: HPCBIOS_2015-01
  * Date of Policy: 2015-02-02

A list has been compiled with the most common compression/decompression tools for Bioinformatics data;

Biocompressors:

+----------------------------------------+-----------------------------+--------------------+------------------------------------------------------------+
| **DSRC**                               | 2.0rc                       | SHOULD             | http://sun.aei.polsl.pl/dsrc                               |
+----------------------------------------+-----------------------------+--------------------+------------------------------------------------------------+
| **fastqz**                             | 1.5                         | SHOULD             | http://mattmahoney.net/dc/fastqz/                          |
+----------------------------------------+-----------------------------+--------------------+------------------------------------------------------------+
| **fqzcomp**                            | 4.6                         | SHOULD             | http://sourceforge.net/projects/fqzcomp/                   |
+----------------------------------------+-----------------------------+--------------------+------------------------------------------------------------+
| **Quip**                               | 1.1.8                       | SHOULD             | http://homes.cs.washington.edu/~dcjones/quip               |
+----------------------------------------+-----------------------------+--------------------+------------------------------------------------------------+
| **SCALCE**                             | 2.7                         | SHOULD             | http://scalce.sourceforge.net/Home                         |
+----------------------------------------+-----------------------------+--------------------+------------------------------------------------------------+
| **ZPAQ**                               | 7.00                        | SHOULD             | http://mattmahoney.net/dc/zpaq.html                        |
+----------------------------------------+-----------------------------+--------------------+------------------------------------------------------------+

Kindly notify -if this policy is inadequate for your work-
both your local site technical representative & HPCBIOS maintainers.

Reference documents:

- Compression of FASTQ and SAM Format Sequencing Data, by James K. Bonfield & Matthew V. Mahoney

  http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0059190

