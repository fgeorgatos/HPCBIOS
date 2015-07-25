.. _HPCBIOS_05-01:

HPCBIOS_05-01: Multiple-Version Software Policy
===============================================

.. note::
  A minimum set of versions of open source and third party software are
  recommended at all HPCBIOS compatible sites.

  * BC Policy: HPCBIOS_05-01
  * Date of Policy: 2012-12-15

These versions are:
  * A primary production version; (MUST)
  * A previous production version, for validation and verification purposes; (SHOULD)
  * Beta or Release-Candidate version to be made available within first month of that release. (MAY)

These three versions MAY vary by package and system,
yet users SHOULD have the ability to test newer versions as they become available
and still have access to production versions.
No attempt/effort will be made to force vendors/upstream providers to provide three versions.

.. seealso::
  The primary concern of this policy is that, when a new production
  version of a package is being deployed at an HPC site it SHALL NOT
  disturb the existing userbase. It remains at site’s discretion to decide
  which version is the current default yet, it SHOULD still allow at least
  one previous production version to serve gracefully users who have
  incompatibilities with newer software and, also allow for testing in advance.
