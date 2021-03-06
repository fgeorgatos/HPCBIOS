.. _HPCBIOS_2012-93: 
HPCBIOS_2012-93: Life Sciences Productivity Environment
================================================================================

.. note::

  Life Sciences Productivity Environment includes a set of HPC tools
  which are needed for scientific computing and visualization in the respective domain. 
  The following is an attempt to define which ones are relevant for the HPCBIOS communities and set an action plan.

  * BC Policy: HPCBIOS_2012-93
  * Date of Policy: 2012-12-15

The main objective of this policy is to provide the following common
productivity environment across any HPCBIOS resources:

+--------------------+------------------------+--------------+--------------------+-------------------------------------------------------------------------------------------+
| Name               | Category               | version(s)   | Compliance level   | Reference URL                                                                             |
+====================+========================+==============+====================+===========================================================================================+
| CPMD               | Quantum Chemistry      | x            | SHOULD             | http://www.cpmd.org/                                                                      |
+--------------------+------------------------+--------------+--------------------+-------------------------------------------------------------------------------------------+
| Dalton             | Quantum Chemistry      | x            | SHOULD             | http://dirac.chem.sdu.dk/daltonprogram.org/                                               |
+--------------------+------------------------+--------------+--------------------+-------------------------------------------------------------------------------------------+
| **GAMESS-US**      | Quantum Chemistry      | x            | SHOULD             | http://www.msg.ameslab.gov/gamess/                                                        |
+--------------------+------------------------+--------------+--------------------+-------------------------------------------------------------------------------------------+
| Gaussian           | Quantum Chemistry      | x            | MAY                | http://www.gaussian.com/                                                                  |
+--------------------+------------------------+--------------+--------------------+-------------------------------------------------------------------------------------------+
| OpenEye            | Chemical Informatics   | x            | SHOULD             | http://www.eyesopen.com/                                                                  |
+--------------------+------------------------+--------------+--------------------+-------------------------------------------------------------------------------------------+
| **BLAST/mpiBLAST** | Sequence Analysis      | x            | MUST               | http://blast.ncbi.nlm.nih.gov/Blast.cgi?CMD=Web&PAGE_TYPE=BlastDocs&DOC_TYPE=Download     |
+--------------------+------------------------+--------------+--------------------+-------------------------------------------------------------------------------------------+
| **BWA**            | Sequence Analysis      | x            | MUST               | http://bio-bwa.sourceforge.net/                                                           |
+--------------------+------------------------+--------------+--------------------+-------------------------------------------------------------------------------------------+
| **CLUSTALW**       | Sequence Analysis      | x            | MUST               | http://www.ebi.ac.uk/Tools/msa/clustalw2/                                                 |
+--------------------+------------------------+--------------+--------------------+-------------------------------------------------------------------------------------------+
| **HMMER**          | Sequence Analysis      | x            | MUST               | http://hmmer.janelia.org/                                                                 |
+--------------------+------------------------+--------------+--------------------+-------------------------------------------------------------------------------------------+
| **MrBayes**        | Sequence Analysis      | x            | MUST               | http://mrbayes.sourceforge.net/                                                           |
+--------------------+------------------------+--------------+--------------------+-------------------------------------------------------------------------------------------+
| **GROMACS**        | Molecular Modeling     | x            | MUST               | http://www.gromacs.org/                                                                   |
+--------------------+------------------------+--------------+--------------------+-------------------------------------------------------------------------------------------+
| **NAMD**           | Molecular Modeling     | x            | SHOULD             | http://www.ks.uiuc.edu/Research/namd/                                                     |
+--------------------+------------------------+--------------+--------------------+-------------------------------------------------------------------------------------------+
| AMBER              | Molecular Modeling     | x            | SHOULD             | http://ambermd.org/                                                                       |
+--------------------+------------------------+--------------+--------------------+-------------------------------------------------------------------------------------------+
| AutoDock /**Vina** | Molecular Modeling     | x            | SHOULD             | http://autodock.scripps.edu/ / http://vina.scripps.edu/                                   |
+--------------------+------------------------+--------------+--------------------+-------------------------------------------------------------------------------------------+
| Glide              | Molecular Modeling     | x            | SHOULD             | http://www.schrodinger.com/                                                               |
+--------------------+------------------------+--------------+--------------------+-------------------------------------------------------------------------------------------+
| **Dock**           | Molecular Modeling     | x            | SHOULD             | http://dock.compbio.ucsf.edu/                                                             |
+--------------------+------------------------+--------------+--------------------+-------------------------------------------------------------------------------------------+
| Flexx              | Molecular Modeling     | x            | SHOULD             | http://www.biosolveit.de/FlexX/                                                           |
+--------------------+------------------------+--------------+--------------------+-------------------------------------------------------------------------------------------+
| FTDock             | Molecular Modeling     | x            | SHOULD             | http://www.sbg.bio.ic.ac.uk/docking/ftdock.html                                           |
+--------------------+------------------------+--------------+--------------------+-------------------------------------------------------------------------------------------+
| LigandFit          | Molecular Modeling     | x            | SHOULD             | http://www.accelrys.com                                                                   |
+--------------------+------------------------+--------------+--------------------+-------------------------------------------------------------------------------------------+
| **Rosetta**        | Molecular Modeling     | 3.5          | SHOULD             | http://www.rosettacommons.org/                                                            |
+--------------------+------------------------+--------------+--------------------+-------------------------------------------------------------------------------------------+

Reference documents:

- PRACE – The Scientific Case for HPC in Europe 2012-2020
  http://www.prace-ri.eu/PRACE-The-Scientific-Case-for-HPC

- European Exascale Software Initiative
  Working Group report on Life Science and Health activities
  http://www.eesi-project.eu/media/download_gallery/EESI_D3.6_WG3.4-Report_R2.0.pdf

This productivity environment may be supplemented with other related
productivity tools as they become available on allocated systems.

Kindly notify -if this policy is inadequate for your work-
both your local site technical representative & HPCBIOS maintainers.
