.. _HPCBIOS_2011-94:

HPCBIOS_2011-94: Bioinformatics & Computational Biology Productivity Environment
================================================================================

.. note::

  Bioinformatics & Computational Biology productivity environment includes a set of HPC tools
  which are needed for scientific computing and visualization in the respective domain. 
  The following is an attempt to define which ones are relevant for the HPCBIOS communities and set an action plan.

  * BC Policy: HPCBIOS_2011-94
  * Date of Policy: 1st December 2012

The main objective of this policy is to provide the following common
productivity environment across any HPCBIOS resources:

+------------+-----------------------+--------------------+--------------------------------------------+
| Name       | Prefered version(s)   | Compliance level   | Reference                                  |
+------------+-----------------------+--------------------+--------------------------------------------+
| R language | v2.7.3                | SHOULD             | http://www.r-project.org                   |
+------------+-----------------------+--------------------+--------------------------------------------+
| *Python* | v2.7.3 | MUST | http://www.python.org/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| *scipy* | 0.10.1 | MUST | http://www.scipy.org/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| *numpy* | 1.6.1 | MUST | http://numpy.scipy.org/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| BioPython | x | SHOULD | http://biopython.org/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| Ruby | v1.9.3-p194 | SHOULD | http://www.python.org/|
+------------+-----------------------+--------------------+--------------------------------------------+
| BioRuby | x | SHOULD | http://bioruby.org/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| Perl | v5.x | SHOULD | http://www.perl.org/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| BioPerl | latest | SHOULD | http://www.bioperl.org/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| Bioconductor| v2.10 | SHOULD | http://www.bioconductor.org/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| *MrBayes* | v3.1.2 | MUST | http://mrbayes.sourceforge.net/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| *AMOS* | 3.1.0 | SHOULD | http://sourceforge.net/apps/mediawiki/amos/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| *Boost* | 1.51 | SHOULD | http://www.boost.org/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| *Bowtie2* | 2.0.0-beta7 | SHOULD | http://bowtie-bio.sourceforge.net/bowtie2 |
+------------+-----------------------+--------------------+--------------------------------------------+
| *BWA* | 0.6.2 | MUST | http://bio-bwa.sourceforge.net/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| *ClustalW2* | 2.1 | MUST | http://www.ebi.ac.uk/Tools/msa/clustalw2/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| *Cufflinks* | 2.0.2 | SHOULD | http://cufflinks.cbcb.umd.edu/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| *Eigen* | 3.1.1 | SHOULD | http://eigen.tuxfamily.org/index.php?title=Main_Page |
+------------+-----------------------+--------------------+--------------------------------------------+
| *FASTX-Toolkit* | 0.0.13.2 | SHOULD | http://hannonlab.cshl.edu/fastx_toolkit/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| *IDBA-UD* | 1.0.9 | SHOULD | http://i.cs.hku.hk/~alse/hkubrg/projects/idba_ud/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| *Infernal* | 1.1rc1 | SHOULD | http://infernal.janelia.org/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| *libgtextutils* | 0.6.1 | SHOULD | http://hannonlab.cshl.edu/fastx_toolkit/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| *MUMmer* | 3.23 | SHOULD | http://mummer.sourceforge.net/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| *MetaVelvet* | 1.2.01 | SHOULD | http://metavelvet.dna.bio.keio.ac.jp/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| *Oases* | 0.2.08 | SHOULD | http://www.ebi.ac.uk/~zerbino/oases/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| *pandaseq* | 2.1 | SHOULD | https://github.com/neufeld/pandaseq |
+------------+-----------------------+--------------------+--------------------------------------------+
| *RNAz* | 2.1 | SHOULD | http://www.tbi.univie.ac.at/~wash/RNAz/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| *SOAPdenovo* | 1.05 | SHOULD | http://soap.genomics.org.cn/index.html |
+------------+-----------------------+--------------------+--------------------------------------------+
| *SAMtools* | 0.1.18 | SHOULD | http://samtools.sourceforge.net/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| *TopHat* | 2.0.4 | SHOULD | http://tophat.cbcb.umd.edu/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| *ViennaRNA* | 2.0.7 | SHOULD | http://www.tbi.univie.ac.at/~ronny/RNA/vrna2.html |
+------------+-----------------------+--------------------+--------------------------------------------+
| *Velvet* | 1.2.07 | SHOULD | http://www.ebi.ac.uk/~zerbino/velvet/ |
+------------+-----------------------+--------------------+--------------------------------------------+
| NCBI toolkit | x | SHOULD | http://www.ncbi.nlm.nih.gov/toolkit |
+------------+-----------------------+--------------------+--------------------------------------------+
| ncbi_blast | x | SHOULD | http://blast.ncbi.nlm.nih.gov/ |
+------------+-----------------------+--------------------+--------------------------------------------+

Future potential candidates for this policy:

+------------+-----------------------+--------------------+--------------------------------------------+
| hmmer | v3 | MUST | http://hmmer.janelia.org/ |
| blast | x | MUST | blast.ncbi.nlm.nih.gov/Blast.cgi?CMD=Web&PAGE_TYPE=BlastDocs&DOC_TYPE=Download |
| mpi-blast | x | MUST | blast.ncbi.nlm.nih.gov/Blast.cgi?CMD=Web&PAGE_TYPE=BlastDocs&DOC_TYPE=Download |
| gpu-blast | x | SHOULD |  |
| cuda-blast | x | SHOULD |  |
| blast+ | x | SHOULD | |
| RAxML | latest | SHOULD | |
| bfast | x | SHOULD | |
| pysam | x | SHOULD | |
| polyphen | x | SHOULD | |
| plink | x | SHOULD | |
| cd-hit | x | SHOULD | |
| readseq | x | SHOULD | |
| meme | x | SHOULD | |
| muscle | x | SHOULD | |
| ssaha | x | SHOULD | |
| repeat masker | x | SHOULD | |
| annovar | x | SHOULD | |
| phrap | x | SHOULD | |
| phred | x | SHOULD | |
| nesoni | x | SHOULD | http://bioinformatics.net.au/software.nesoni.shtml |
| MCL | x | SHOULD |  |
| cython | 0.16 | SHOULD | |
| phyml_v3 | x | SHOULD | |
| paul | x | SHOULD | |
| consed | x | SHOULD | |
| galaxy | >ca0c4ad2bb39 | SHOULD | http://galaxy.psu.edu/ |
| cigri | v3 | SHOULD | http://cigri.imag.fr/ |
+------------+-----------------------+--------------------+--------------------------------------------+

This productivity environment will be supplemented with other related
productivity tools as they become available on allocated systems.

Potential sources of information for future upgrades of this list include:
* http://www.vital-it.ch/software/tools.php
* http://www.csc.fi/english/research/sciences/bioscience/programs/index_html
* http://bacpathgenomics.wordpress.com/software/
* http://umbc.rnet.missouri.edu/general/software/alphabetical.html
* http://www.broadinstitute.org/software/bsi-sig/
* http://ncgas.org/software,%20genome%20assembly,%20assembly,%20genomics
* http://confluence.rcs.griffith.edu.au:8080/display/GHPC/qiime#qiime-Alignment%2Ctreebuilding%2Ctaxonomyassignment%2COTUpicking%2Candotherdatagenerationsteps%28requiredforalternativepipelines%29
* http://www.bioplexity.org/lectures/ebi-s10.pdf

Kindly notify -if this policy is inadequate for your work-
both your local site technical representative & HPCBIOS user-support.

