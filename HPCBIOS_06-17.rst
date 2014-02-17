.. _HPCBIOS_06-17:

HPCBIOS_06-17: Use of Modules for Accessing Multiple Versions of Software
=========================================================================

.. note::
  Any compliant system is required to install and use an ENVIRONMENT MODULES
  package to support multiple versions of compilers, associated libraries,
  and heavily used application software (fi. OpenMPI, NetCDF, WRF, WIEN2K et al)
  on the available resources of HPC sites. Compliance is determined by
  sites ensuring that the *module* command is in the user’s path and that
  system modulefiles are possible to provide for (the subset of) software packages
  mentioned above that are supported by each site.

  * BC Policy: HPCBIOS_06–17
  * Date of Policy: 2012-12-15

The ENVIRONMENT MODULES package provides for the dynamic modification of
a user’s environment via modulefiles. Each modulefile contains the information
needed to configure the shell environment for an application. Once the
Modules package is initialized, the environment can be modified on a
per-module basis using the module command which interprets modulefiles.

Typically, modulefiles instruct the module command to alter or set shell
environment variables such as PATH, MANPATH, tune aliases etc. Modulefiles may be
shared by many users on a system and users may have their own collection
to supplement or replace the shared modulefiles.

Scope
-----

ENVIRONMENT MODULES can be loaded and unloaded dynamically and atomically in a clean
fashion. Common shells like bash, sh, tcsh, csh MUST be supported - while
ksh, zsh (Ref: |HPCBIOS_05-06|), as well as some scripting languages such as
Perl (Ref: |HPCBIOS_06-04|) MAY be supported, as per each site's needs/capabilities.

Implementation
--------------

The function of the modulefiles is to modify a user’s environment such
that a user references the selected version of an application using
the default commands for that application without hardcoding paths
or version information. This allows to maximize code reuse and
pave the way for uniform documentation across software versions.

Implementations that are known to be compliant are:

* *environment-modules-c*
* *environment-modules-tcl*
* *Lmod*

The individual site MAY combine
compliant modulefiles with other existing site-specific methods (e.g. additional
modulefiles or wrapper scripts) to select versions of applications
t help define the user’s environment (fi. storage locations, project variables etc).

Dependencies
------------

In the cases where the modulefiles for applications depend on other
modulefiles (an application may require compiler and library modulefiles
to be loaded), these dependencies SHOULD be checked, upon load. A reasonably
default modulefile MAY be loaded, if the dependency is not met already.

A site MAY automatically unload dependencies of a given modulefile, upon unload.
Note that different user communities could well have different valid reasons
for or against the default attitude upon unloading, therefor this is deliberately left open.

Escape path
-----------

An additional modulefile MAY exist, called OPT-OUT, which will remove
the system's common-link directories from the associated *PATH* environment variables. Users will
then need to load individual modulefiles to add the application specific
directories to the PATH environment variables.

.. seealso::
  The currently recommended namespace format is the one provided via EasyBuild v1.11 (see |HPCBIOS_2012-92|),
  and a site MAY use aliases for default modules, as defined via UNITE, version May 2010.
  UNITE suite provides definitions with examples under section 1.2 of its documentation:
  http://apps.fz-juelich.de/unite/files/unite-installguide.pdf

.. |HPCBIOS_05-06| replace:: [:ref:`HPCBIOS_05-06 <HPCBIOS_05-06>`]
.. |HPCBIOS_06-04| replace:: [:ref:`HPCBIOS_06-04 <HPCBIOS_06-04>`]
.. |HPCBIOS_2012-92| replace:: [:ref:`HPCBIOS_2012-92 <HPCBIOS_2012-92>`]
