.. _HPCBIOS_10-02:

HPCBIOS_10-02: Common Open Source High Productivity Languages
=============================================================

.. note::
  High Productivity Languages have recently become an important part of
  scientific computing and visualization environment. Leading high productivity
  languages include R, the commercially available MATLAB, open source Python
  (with its scientific computing add-ons) and open source Octave.

  Each of these high productivity languages forms an integral part of a standard
  library that includes text processing, file I/O, data compression, and a
  host of capabilities ranging from basic numerical linear algebra to complex data
  visualization. As such they are an indispensable component of any modern HPC platform.

  * BC Policy: HPCBIOS_10-02
  * Date of Policy: 2012-12-15

The main objective of this policy is to provide the following common
open source high productivity languages environment across all HPCBIOS compliant resources:

+----------------+-------------------------------------------------+--------------------+------------------------------------------+
| Package/Tool   | Description                                     | Compliance level   | Reference                                |
+================+=================================================+====================+==========================================+
| **Python**     | General Purpose Scripting Language              | MUST               | http://python.org/                       |
+----------------+-------------------------------------------------+--------------------+------------------------------------------+
| **NumPy**      | Numerical Arrays and Linear Algebra in Python   | MUST               | http://numpy.scipy.org/                  |
+----------------+-------------------------------------------------+--------------------+------------------------------------------+
| **SciPy**      | Scientific Python                               | MUST               | http://www.scipy.org/                    |
+----------------+-------------------------------------------------+--------------------+------------------------------------------+
| PyMPI          | Python Message Passing Interface                | SHOULD             | http://pympi.sourceforge.net/            |
+----------------+-------------------------------------------------+--------------------+------------------------------------------+
| **Octave**     | MATLAB Clone                                    | MUST               | http://www.gnu.org/software/octave/      |
+----------------+-------------------------------------------------+--------------------+------------------------------------------+
| **matplotlib** | Scientific 2-D and 3-D Plotting                 | MUST               | http://matplotlib.sourceforge.net/       |
+----------------+-------------------------------------------------+--------------------+------------------------------------------+
| **R**          | R language                                      | MUST               | http://www.r-project.org/                |
+----------------+-------------------------------------------------+--------------------+------------------------------------------+
| **MATLAB**     | MATLAB is a high-level language for computation | SHOULD (commercial)| http://www.mathworks.nl/products/matlab/ |
+----------------+-------------------------------------------------+--------------------+------------------------------------------+
| NAG            | Numerical library /Numerical Algorithms Group   | SHOULD (commercial)| http://www.nag.co.uk/                    |
+----------------+-------------------------------------------------+--------------------+------------------------------------------+

This high productivity languages environment will be supplemented with
more open source productivity languages, as they become available on allocated systems.

There are three key sources which MAY be used to provide support to the
scripting language Python and its scientific add-ons NumPy, PyMPI and SciPy,
as well as more tools from the above list. These are:

- EasyBuild. See policy |HPCBIOS_2012-92| ; in fact, this is the preferred way,
  since integration with the other scientific software is better guaranteed.

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

At least one of EasyBuild, CSE or PToolsRTE, SHOULD be made available on HPC systems.

EasyBuild is maintained by *Ghent University* and is available as open source python codebase,
while the CSE package is being maintained by the *ARL CSE* Team
and the PToolsRTE is being maintained through *PETTT* project.
Sites are encouraged to used reproducible techniques for herding software components!

.. |HPCBIOS_2012-92| replace:: [:ref:`HPCBIOS_2012-92 <HPCBIOS_2012-92>`]

