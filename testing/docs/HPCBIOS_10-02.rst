HPCBIOS_10-02: Common Open Source High Productivity Languages
==============================================

.. note::
  High productivity languages have recently become an important part of
  scientific computing and visualization. Leading high productivity
  languages include the commercially available MATLAB, open source Python
  (with its scientific computing add-ons) and open source Octave. Each of
  these high productivity languages forms an integral part of a standard
  library that includes text processing, file I/O, data compression, and a
  host of capabilities ranging from basic numerical linear algebra to
  complex data visualization.

  * BC Policy: HPCBIOS_10-02
  * Date of Policy: 1st November 2012

The main objective of this policy is to provide the following common
open source high productivity languages environment across all HPCBIOS
compliant resources:

+----------------+-------------------------------------------------+--------------------+------------------------------------------+
| Package/Tool   | Description                                     | Compliance level   | Reference                                |
+----------------+-------------------------------------------------+--------------------+------------------------------------------+
| Python         | General Purpose Scripting Language              | MUST               | `http://python.org/`_                    |
+----------------+-------------------------------------------------+--------------------+------------------------------------------+
| NumPy          | Numerical Arrays and Linear Algebra in Python   | MUST               | `http://numpy.scipy.org/`_               |
+----------------+-------------------------------------------------+--------------------+------------------------------------------+
| PyMPI          | Python Message Passing Interface                | MUST               | `http://pympi.sourceforge.net/`_         |
+----------------+-------------------------------------------------+--------------------+------------------------------------------+
| SciPy          | Scientific Python                               | MUST               | `http://www.scipy.org/`_                 |
+----------------+-------------------------------------------------+--------------------+------------------------------------------+
| Octave         | MATLAB Clone                                    | SHOULD             | `http://www.gnu.org/software/octave/`_   |
+----------------+-------------------------------------------------+--------------------+------------------------------------------+
| Matplotlib     | Scientific 2-D and 3-D Plotting                 | SHOULD             | `http://matplotlib.sourceforge.net/`_    |
+----------------+-------------------------------------------------+--------------------+------------------------------------------+
| NAG            | Numerical library /Numerical Algorithms Group   | SHOULD             | `http://www.nag.co.uk/`_                 |
+----------------+-------------------------------------------------+--------------------+------------------------------------------+
| R              | R language                                      | SHOULD             | `http://www.r-project.org/`_             |
+----------------+-------------------------------------------------+--------------------+------------------------------------------+

These high productivity languages environment will be supplemented with
other open source productivity languages as they become available on
allocated systems.

There are two key sources which MAY be used to provide support to the
scripting language Python and its scientific add-ons NumPy, PyMPI and
SciPy. These are:

- Computational Science Environment (CSE). The CSE is an integrated
production level environment developed at *ARL DSRC*. CSE consists of
open source tools, libraries as well as Python support (Python, NumPy,
SciPy and PyMPI). All CSE components are assembled in an extensible
framework that handles software dependencies at compile and runtime.

- Parallel Tools Runtime Environment (PToolsRTE). The PToolsRTE is a
collection of Python, NumPy, PyMPI, SciPy and related packages,
including Matplotlib, developed by ParaTools, Inc. PToolsRTE provides a
hybrid binary and source distribution where a majority of the components
are pre-packaged in a binary form and a minimal number of platform and
compiler specific components are built on the target system. This
simplifies the complexity of software installation and the runtime
environment can be easily installed on external systems to provide a
consistent Python based environment for developing and deploying
scientific packages that rely on a common runtime environment.

Both the CSE and PToolsRTE MAY be made available on HPC systems. The CSE
package is being maintained by the *ARL CSE* Team, while the PToolsRTE
is being maintained through *PETTT*.
