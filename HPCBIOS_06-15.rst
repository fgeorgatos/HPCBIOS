.. _HPCBIOS_06-15:

HPCBIOS_06-15: Sample Code Repository
========================================

.. note::
  Each compatible site shall maintain a user-accessible Sample Code
  Repository of frequently-used procedures, routines, scripts, and codes
  on each project affiliated system. Users of all skill levels can use the
  samples in the Repository to find best practices for various situations.
  The samples will be especially helpful to users who are new to
  HPCBIOS sites or to a particular system.

  * BC Policy: HPCBIOS_06–15
  * Date of Policy: 2012-12-15

An environment variable named $SAMPLES_HOME will point to the
Repository base directory. Each sample will be findable via its own
subdirectory under the base directory. The exact architecture of the
sample directories and the formatting style of the contents will be left
to the discretion of the sites. However, each sample, including all
scripts, codes, Makefiles, etc., shall be well-documented
and shall be as self-contained as possible.

The top-level $SAMPLES_HOME directory shall contain an index file named
INDEX.txt. This file includes the name and a brief explanation of each
sample. The entries in the index file shall be organized by category.
A description of the Code Repository and the INDEX.txt listing from each
system shall be placed on the site’s website or other suitable documentation area.

Samples in the Repository will be created primarily by each site’s staff.
However, a site may choose to allow users to submit prospective
samples for consideration as new entries in the Repository, subject to
approval by the site staff. The submitting user shall provide all
necessary files and documentation, as well as future updates.
Site staff shall be responsible for placing new samples and updates into the Repository.

In addition to the above-mentioned samples, each site may also have a
collection of simple, stand-alone tools and scripts for the convenience
of users of the systems. The tools and scripts, if present,
shall be available in the users' default search path or, retrievable via modules.

The $SAMPLES_HOME directory shall contain a text file named
AVAILABLE_TOOLS.txt. This file will contain a list of the tools that
are available on the machine on which the file is stored. In addition to
listing the tools, a short description of each will be provided.
If there is no man page available for a particular tool, then a description
on how to use that tool will be included in the listing file.

If a site has no such tools for a particular resource,
the AVAILABLE_TOOLS.txt file must still exist, and it must specify that no
such tools are available for that resource.

