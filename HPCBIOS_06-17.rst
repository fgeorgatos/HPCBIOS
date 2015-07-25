.. _HPCBIOS_06-17:

HPCBIOS_06-17: Use of Modules for Accessing Multiple Versions of Software
=========================================================================

.. note::
  Use of environment modules is the standard technology on HPC sites
  for handling multiple software versions, in a manner which offers orthogonality.

  Any compliant system is required to install and use some ENVIRONMENT MODULES
  technology to support multiple versions of compilers, associated libraries,
  and heavily used application software (fi. OpenMPI, HDF5, NetCDF, WRF et al)
  on the available resources of HPC sites. Compliance is determined by
  sites ensuring that the *module* command is in the users' path and that
  modulefiles available by support staff are accessible in some way.

  * BC Policy: HPCBIOS_06–17
  * Date of Policy: 2012-12-15

The ENVIRONMENT MODULES package provides for the dynamic modification of
a user’s environment via modulefiles. Each modulefile contains the information
needed to configure the shell environment for an application. Once the
Modules package is initialized, the environment can be modified on a
per-module basis, using the module command which interprets modulefiles.

Typically, modulefiles instruct the module command to alter or set shell
environment variables such as PATH, MANPATH, define aliases etc.
Modulefiles may be shared by many users on a system and users may have
their own collection to supplement or replace the shared modulefiles.

Scope
-----

ENVIRONMENT MODULES can be loaded and unloaded dynamically and atomically in a clean fashion.
Common shells such as bash, sh, tcsh/csh MUST be supported - while
ksh, zsh (Ref: |HPCBIOS_05-06|), as well as some scripting languages such as
Python or Perl (Ref: |HPCBIOS_06-04|) MAY be supported, as per each site's needs/capabilities.

Implementation
--------------

The function of the modulefiles is to modify a user’s environment such
that a user may reference the selected version of an application using
the default commands for that application without hardcoding paths
or version information. This allows to maximize code reuse
and pave the way for uniform documentation across software versions.

Implementations which are known to be compliant with the above needs are:

* *environment-modules-c*   # version >= 3.2.10
* *environment-modules-tcl* # version >= 1.562
* *Lmod*                    # version >= 5.9.0

The individual site MAY combine compliant environment modules implementations
and modulefiles with more existing site-specific methods (e.g. additional
modulefiles or profile initialization or wrapper scripts) to select versions of applications
to help define the user’s environment (fi. storage locations, project variables etc).

Dependencies
------------

In the cases where the modulefiles for applications depend on other
modulefiles (an application may require compiler and library modulefiles
to be loaded), these dependencies SHOULD be controlled, upon load time.
A reasonably default modulefile MAY be loaded, if the dependency is not met already.

A site MAY automatically unload dependencies of a given modulefile, upon unload.
Note that different user communities COULD well have different valid reasons
for or against the default attitude upon unloading, therefor this is deliberately left open.

Escape path
-----------

An additional modulefile MAY exist, called OPT-OUT, which will remove
the system's common-link directories from the associated *PATH* environment variables.
Users will then need to load individual modulefiles to add the application specific
directories to the PATH environment variables.

.. seealso::
  The currently suggested namespace format is the one provided via EasyBuild v2 (see |HPCBIOS_2012-92|),
  and a site MAY use aliases for default modules, as defined via UNITE, version May 2010.
  UNITE suite provides definitions with examples under section 1.2 of its documentation:
  http://apps.fz-juelich.de/unite/files/unite-installguide.pdf
  The above namespaces are essentially *flat*, meanwhile sites MAY prefer *hierarchical* namespaces.

.. |HPCBIOS_05-06| replace:: [:ref:`HPCBIOS_05-06 <HPCBIOS_05-06>`]
.. |HPCBIOS_06-04| replace:: [:ref:`HPCBIOS_06-04 <HPCBIOS_06-04>`]
.. |HPCBIOS_2012-92| replace:: [:ref:`HPCBIOS_2012-92 <HPCBIOS_2012-92>`]

