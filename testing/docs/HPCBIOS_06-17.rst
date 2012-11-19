.. _HPCBIOS_06-17:

HPCBIOS_06-17: Use of Modules for Accessing Multiple Versions of Software
=========================================================================

.. note::
  All participating centers are required to install and use the MODULES
  package to support multiple versions of compilers, associated libraries,
  and heavily used application software (netcdf, openmpi, wrf, wien2k et al)
  on the available resources of HPC sites. Compliance is determined by
  centers ensuring that the modules command is in the user’s path and that
  system modulefiles are in place for the software packages mentioned
  above that are supported by the center.

  * BC Policy: HPCBIOS_06–17
  * Date of Policy: 1st November 2012

The MODULES package provides for the dynamic modification of a user’s
environment via modulefiles. Each modulefile contains the information
needed to configure the shell environment for an application. Once the
Modules package is initialized, the environment can be modified on a
per-module basis using the module command which interprets modulefiles.
Typically, modulefiles instruct the module command to alter or set shell
environment variables such as PATH, MANPATH, etc. Modulefiles may be
shared by many users on a system and users may have their own collection
to supplement or replace the shared modulefiles.

## Scope

MODULES can be loaded and unloaded dynamically and atomically in a clean
fashion. Popular shells like bash, sh, tcsh, csh MUST be supported - while
ksh, zsh (Ref: |HPCBIOS_05-06|) as well as some scripting languages such as
Perl (Ref: |HPCBIOS_06-04|) MAY be supported.

## Implementation

The function of the modulefiles is to modify a user’s environment such
that the user references the selected version of an application using
the default commands for that application without adding additional path
or version information. The individual center may combine these
compliant modulefiles with existing methods (e.g. additional
modulefiles, wrapper scripts) to select versions of applications and
modify the user’s environment.

## Dependencies

In the cases where the modulefiles for applications depend on other
modulefiles (an application may require compiler and library modulefiles
to be loaded), these dependencies should be checked. A reasonable
default modulefile shall be loaded if the dependency is not met.

## Escape path

An additional modulefile SHOULD exist, called OPT-OUT, which will remove the common-link
directories from the associated **PATH environment variables. Users will
then need to load individual modulefiles to add the application specific
directories to the PATH environment variables**.

.. seealso::
  The currently preferred namespace format is the one provided via EasyBuild v1.0,
  with potential aliases for default modules as defined via UNITE version May 2010.
  UNITE suite provides definitions under section 1.2 of its documentation:
  http://apps.fz-juelich.de/unite/files/unite-installguide.pdf


.. |HPCBIOS_05-06| replace:: [:ref:`HPCBIOS_05-06 <HPCBIOS_05-06>`]
.. |HPCBIOS_06-04| replace:: [:ref:`HPCBIOS_06-04 <HPCBIOS_06-04>`]
