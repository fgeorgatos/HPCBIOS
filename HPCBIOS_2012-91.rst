.. _HPCBIOS_2012-91:

HPCBIOS_2012-91: Modules Namespace for HPC sites
================================================

.. note::

  The main objective of this policy is to provide a consistent module namespace across any HPCBIOS compatible resources.

  * BC Policy: HPCBIOS_2012-91
  * Date of Policy: 2012-12-15


Description
-----------

This document specifies a syntax for defining the names of packages as
they become available via the modules mechanism of HPC sites. Such
definition is important when sites perform under a common project or,
share their user base or. simply, systems administrators need to swap configuration.

The key words “MUST”, “MUST NOT”, “REQUIRED”, “SHALL”, “SHALL NOT”,
“SHOULD”, “SHOULD NOT”, “RECOMMENDED”, “MAY”, and “OPTIONAL” in this
document are to be interpreted as described in :rfc:`2119`.

Introduction
------------

When the users enter an HPC system, they need to tune their software
environment variables (to find available programs, library & include
paths etc). The most common solution for that issue has been modules_ ;
In practice though, HPC sites act in isolation, with lots of
divergence in their module namespace. This does not allow good training
examples or working code reuse by users so, work has to be done to bring
convergence of the namespace across HPC sites.

This document is an attempt to define basic guidelines for modules
namespace in order to address homegeneity arguments and reduce maintenance effort.

Scope
-----

The standard should capture the maximum possible compatibility across sites,
reducing unnecessary divergence, yet being practical and allowing
some flexibility for local HPC sites needs & policies. There is a
deliberate effort to be compatible with existing PRACE_ , DEISA_ , UNITE_ & PARMA-ITEA2_ guidelines.

Standard to follow
------------------

The following approach is being suggested:

Package Lists and software guidelines:

- Any Package List SHOULD supply Package names in a non-ambiguous case-sensitive format
- The case-sensitive Package name SHOULD be derived from software author's naming preference

Conforming sites SHOULD adhere to these principles:

- MUST provide either the original Package name or, the lower case version
- MUST place the Version string after the “/” separator (to permit operation *module swap*)
- MUST document their module configuration & namespace policy, explicitly
- SHOULD provide a default Version when multiple ones exist (or, let one be implied)
- SHOULD prefer numbered Version strings with dots notation (as opposed to _ or - separators)
- MAY further expand the Version string or provide aliases, as per local needs;
  - examples: ``-goolf-*``, ``-openmpi-intel-32bit``
- MAY provide multiple buildsets of modules, as per local needs;
  - examples: ``HPCBIOS.20130902``, ``HPCBIOS.20131224``
- MAY provide multiple subcategories of modules, as per local needs;
  - examples: ``bio cae chem compiler debugger devel ide lib math mpi numlib performance phys system tools vis``

For sites planning to be conforming to this standard,
it is very important to adhere at the stated requirement levels
and rigidly document implementation and deviations,
so that users receive little to no surprise when moving from site to site.

Definitions
-----------

If definitions are required for what some terms mean, they can be considered as defined
via UNITE standard (p.2/1.2) The relevant text is copied hereby, with only minor adjustments:

Package
  A software product, tool, or component which has its own name, a
  specific source and, is available / can be used / can be installed as
  separate entity.

Version
  Basic version naming SHOULD be in the form ``<MajorVersion>.<MinorVersion>``
  or ``<MajorVersion>.<MinorVersion>.<PatchLevel>`` optionally followed by
  either ``b<Number>`` in case of a beta version or ``rc<Number>`` for
  release candidates. Examples: ``2.1, 4.1.3, 3.2b2, 4.5rc1``

Specialization
  Optional constraints which limit the applicability of a version of a package.
  Example: ``WRF/3.3.1-goolf-1.4.10-dmpar`` (ie. the suffix after the version)
  This MAY be necessary on computing systems which provide multiple MPI libraries
  or compiler suites (e.g., very commonly on Linux clusters). The alias of the
  default version MAY take the form ``-<MPILibrary>-<Compiler>-<Precision>``.
  If so, the three components MUST always be specified in this order,
  however unnecessary constraints (not provided by a system) can be left out.
  Examples: ``-openmpi-64bit`` , ``-mvapich-gnu-32bit`` etc

Fully-Qualified Version (FQV)
  A fully-qualified version is the complete specification of a version
  of a package installed under specific constraints, i.e., it is the
  combination of a version followed by a specialization separated by a
  dash (“-”). Example: ``1.4.3-mpich2-intel``.

Platform
  The target computer system on which Package is installed. A platform
  is characterized by its vendor, architecture, and set of compiler suites
  and MPI libraries available for parallel programming.


References
----------

-  http://modules.sourceforge.net/
-  http://apps.fz-juelich.de/unite/files/unite-installguide.pdf
-  http://www.deisa.eu/usersupport/user-documentation/deisa-common-production-environment/modules-usage
-  http://www.deisa.eu/usersupport/user-documentation/deisa-common-production-environment/deisa-common-production-environment.pdf
-  http://www.prace-ri.eu/prace-common-production/

Kindly notify -if this policy is inadequate for your work-
both your local site technical representative & HPCBIOS maintainers.


.. _modules: http://modules.sourceforge.net/
.. _DEISA: http://www.deisa.eu/usersupport/user-documentation/deisa-common-production-environment/deisa-common-production-environment.pdf
.. _PRACE: http://www.prace-ri.eu/prace-common-production/
.. _UNITE: http://apps.fz-juelich.de/unite/files/unite-installguide.pdf
.. _PARMA-ITEA2: http://www.parma-itea2.org/

