.. _HPCBIOS_2012-80:

HPCBIOS_2012-96: Common Set of DFT codes
========================================

.. note::

  Providing (a subset of) popular DFT codes is nearly imperative for most HPC centers.
  This is an work-in-progress effort to provide the candidate list as a set.
  There is no particular level of compliance as of yet (all list is "SHOULD" status).

  * BC Policy: HPCBIOS_2012-96
  * Date of Policy: 20121212

Introduction
------------

The following is a list of sites that document
various density-functional theory based electronic structure codes,
both periodic and molecular, and atomic pseudopotential codes.
This list is no way comprehensive,
nor makes any representation of what the codes do, beyond the most
superficial observations (being predominantly a molecular code
vs. being predominantly a periodic code, local orbital vs. plane wave).
The principal distinction of items on this list is that I ran
across the web site when looking for other things on the
web, I had heard of them at some point in the literature, and, at the
time I discovered them, the web site appeared to be functioning.
We welcome suggestions of additions and corrections.

DFT production codes
--------------------

Periodic codes (mainly)
~~~~~~~~~~~~~~~~~~~~~~~

Plane wave and related methods
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

+----------------------------------------------------------------------+------------------------+
|  http://cms.mpi.univie.ac.at/vasp                                    | VASP                   |
+----------------------------------------------------------------------+------------------------+
|  http://www.tcm.phy.cam.ac.uk/castep                                 | CASTEP and CETEP       |
+----------------------------------------------------------------------+------------------------+
|  http://www.cpmd.org                                                 | CPMD                   |
+----------------------------------------------------------------------+------------------------+
|  http://www.abinit.org                                               | **ABINIT**             |
+----------------------------------------------------------------------+------------------------+
|  http://inac.cea.fr/L_Sim/BigDFT                                     | BigDFT                 |
+----------------------------------------------------------------------+------------------------+
|  http://www.quantum-espresso.org                                     | **Quantum-Espresso**   |
+----------------------------------------------------------------------+------------------------+
|  http://www.nersc.gov/~linwang/PEtot/PEtot.html                      | PEtot                  |
+----------------------------------------------------------------------+------------------------+
|  https://wiki.fysik.dtu.dk/dacapo                                    | DACAPO                 |
+----------------------------------------------------------------------+------------------------+
|  http://dft.sandia.gov/Socorro/mainpage.html                         | Socorro                |
+----------------------------------------------------------------------+------------------------+
|  http://dft.physics.cornell.edu                                      | DFT++                  |
+----------------------------------------------------------------------+------------------------+
|  http://www.tddft.org/programs/octopus                               | Octopus                |
+----------------------------------------------------------------------+------------------------+
|  http://www.nersc.gov/projects/paratec                               | Paratec                |
+----------------------------------------------------------------------+------------------------+
|  http://cst-www.nrl.navy.mil/people/singh/planewave/v3.0             | DoD Planewave          |
+----------------------------------------------------------------------+------------------------+
|  http://www.ices.utexas.edu/parsec                                   | PARSEC                 |
+----------------------------------------------------------------------+------------------------+
|  http://cp2k.berlios.de                                              | **CP2K**               |
+----------------------------------------------------------------------+------------------------+
|  https://wiki.fysik.dtu.dk/gpaw                                      | **GPAW**               |
+----------------------------------------------------------------------+------------------------+
|  http://www.sphinxlib.de                                             | SPHINX                 |
+----------------------------------------------------------------------+------------------------+
|  http://eslab.ucdavis.edu/software/qbox                              | QBOX                   |
+----------------------------------------------------------------------+------------------------+

Local orbital basis codes
^^^^^^^^^^^^^^^^^^^^^^^^^

+----------------------------------------------------------------------+------------------------+
|  http://dft.sandia.gov/Quest                                         | Quest                  |
+----------------------------------------------------------------------+------------------------+
|  http://www.cs.sandia.gov/~paschul/Quest                             | SeqQuest               |
+----------------------------------------------------------------------+------------------------+
|  http://www.icmab.es/siesta                                          | SIESTA                 |
+----------------------------------------------------------------------+------------------------+
|  http://www.cse.dl.ac.uk/Activity/CRYSTAL                            | CRYSTAL - CSE          |
+----------------------------------------------------------------------+------------------------+
|  http://aimpro.ncl.ac.uk                                             | AIMPRO                 |
+----------------------------------------------------------------------+------------------------+
|  http://www.fplo.de                                                  | FPLO                   |
+----------------------------------------------------------------------+------------------------+
|  http://www.openmx-square.org                                        | OpenMX                 |
+----------------------------------------------------------------------+------------------------+

All-electron (augmented methods) codes
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

+----------------------------------------------------------------------+------------------------+
|  http://elk.sourceforge.net                                          | ELK                    |
+----------------------------------------------------------------------+------------------------+
|  http://exciting-code.org                                            | EXCITING               |
+----------------------------------------------------------------------+------------------------+
|  http://www.flapw.de                                                 | FLEUR                  |
+----------------------------------------------------------------------+------------------------+
|  http://www.rspt.net                                                 | RSPt                   |
+----------------------------------------------------------------------+------------------------+
|  http://www.wien2k.at                                                | **WIEN2k**             |
+----------------------------------------------------------------------+------------------------+

Molecular codes
~~~~~~~~~~~~~~~

+----------------------------------------------------------------------+------------------------+
|  http://www.gaussian.com                                             | Gaussian               |
+----------------------------------------------------------------------+------------------------+
|  http://www.emsl.pnl.gov/docs/nwchem/nwchem.html                     | NWChem                 |
+----------------------------------------------------------------------+------------------------+
|  http://people.web.psi.ch/delley/dmol3.html                          | DMol3                  |
+----------------------------------------------------------------------+------------------------+
|  http://www.schrodinger.com/Products/jaguar.html                     | Jaguar                 |
+----------------------------------------------------------------------+------------------------+
|  http://www.msg.chem.iastate.edu/gamess                              | GAMESS                 |
+----------------------------------------------------------------------+------------------------+
|  http://www.q-chem.com                                               | QCHEM                  |
+----------------------------------------------------------------------+------------------------+
|  http://quantum.utep.edu/nrlmol/nrlmol.html                          | NRLMOL                 |
+----------------------------------------------------------------------+------------------------+
|  http://www.t12.lanl.gov/home/mchalla                                | MondoSCF               |
+----------------------------------------------------------------------+------------------------+
|  http://www.scm.com                                                  | ADF - SCM              |
+----------------------------------------------------------------------+------------------------+
|  http://www.demon-software.com                                       | deMon                  |
+----------------------------------------------------------------------+------------------------+
|  http://www-theor.ch.cam.ac.uk/software/caddoc.html                  | CADPAC                 |
+----------------------------------------------------------------------+------------------------+
|  http://pyquante.sourceforge.net                                     | PYQUANTE               |
+----------------------------------------------------------------------+------------------------+
|  http://www.cosmologic.de/QuantumChemistry/main_qChemistry.html      | TURBOMOLE              |
+----------------------------------------------------------------------+------------------------+

DFT atomic pseudopotential codes
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

+----------------------------------------------------------------------+------------------------+
|  http://www.fhi-berlin.mpg.de/th/fhi98md/fhi98PP                     | fhi98PP                |
+----------------------------------------------------------------------+------------------------+
|  http://opium.sourceforge.net                                        | OPIUM                  |
+----------------------------------------------------------------------+------------------------+
|  http://www.tddft.org/programs/APE                                   | APE                    |
+----------------------------------------------------------------------+------------------------+
|  http://www.physics.rutgers.edu/~dhv/uspp                            | USPP                   |
+----------------------------------------------------------------------+------------------------+
|  http://www.openmx-square.org/adpack/adpack.html                     | ADPACK                 |
+----------------------------------------------------------------------+------------------------+
|  http://www.wfu.edu/~natalie/papers/pwpaw/man.html                   | ATOMPAW                |
+----------------------------------------------------------------------+------------------------+
|  http://www.nnin.org/nnin_comp_psp_vault.html                        | Virtual Vault for PP   |
+----------------------------------------------------------------------+------------------------+

DFT functionals
~~~~~~~~~~~~~~~

+----------------------------------------------------------------------+------------------------+
|  http://dft.sandia.gov/functionals/AM05.html                         | AM05                   |
+----------------------------------------------------------------------+------------------------+
|  http://dft.uci.edu/pubs/PBE.asc                                     | PBE                    |
+----------------------------------------------------------------------+------------------------+
|  http://dft.uci.edu/pubs/PBEsol.html                                 | PBEsol                 |
+----------------------------------------------------------------------+------------------------+
|  http://comp.chem.umn.edu/info/dft.htm                               | Truhlar functionals    |
+----------------------------------------------------------------------+------------------------+
|  http://www.tddft.org/programs/octopus/wiki/index.php/Libxc          | Libxc                  |
+----------------------------------------------------------------------+------------------------+

Useful links
------------

 * http://dft.sandia.gov/Quest/DFT_codes.html
 * http://en.wikipedia.org/wiki/List_of_quantum_chemistry_and_solid-state_physics_software

.. note::

  The current form of the policy currently does not specify 32 bit vs 64
  bit version, though it is expected that the native architecture of a
  given system (typically 64 bits) is supported as the default target,
  while the other is optional but desired to have (typically 32 bits).

