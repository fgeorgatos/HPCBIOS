.. _HPCBIOS_05-06:

HPCBIOS_05-06: Baseline Set of Login Shells
===========================================

.. note::
  A user MAY specify any login shell among the Login Shells baseline set
  as the default shell, via a new user application.

  * BC Policy: HPCBIOS_05-06
  * Date of Policy: 2012-12-15

Sites MAY provide their users with login shell choices beyond this list,
but all sites MUST provide every login shell in the current baseline set.

Users MAY request a change to the current login shell for
their active accounts at any site via email, telephone, or walk-in request.

This policy is not a guarantee that all shells will be working under all
circumstances (fi. in a modulefiles context) or, that a particular version will be available.

Sites MAY force changes in available shell versions, due to security or other operational needs.

Sites MAY opt to use modules for providing certain shell/version combinations.

Sites MAY choose to restrict users from changing default login shells,
esp. if these are not originally specified during allocation application.
(ie. specific dependencies on shells MUST be declared and tested in advance, before
a large allocation is made. Users are advised to test their codes under a preparatory scheme)

The Login Shells baseline set and user selection policy MAY vary;
in that case it MUST be documented at each site’s website or system (fi. MOTD).

Default Login Shell Baseline Set
  * Bourne (sh)
  * Korn (ksh)
  * C shell (csh)
  * Extended C-shell (tcsh)
  * GNU Bourne-again shell (bash)
  * Z shell (zsh)
