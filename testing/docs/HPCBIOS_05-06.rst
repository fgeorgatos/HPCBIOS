HPCBIOS_05-06: Baseline Set of Login Shells
===========================================

.. note::
  A user MAY specify any login shell of the login shell baseline as the
  default shell on a new user application.

  * BC Policy: HPCBIOS_05-06
  * Date of Policy: 1st November 2012

Centers MAY provide their users login shell choices beyond the login
shell baseline, but all centers SHOULD provide every login shell in the
baseline set. Users MAY request a change to the current login shell for
their active accounts at any center via email, telephone, or walk-in
request.

This policy is not a guarantee that all shells will be working under all
circumstances (eg. modules) or, that a particular version will be available.

Centers MAY choose to restrict users from changing login shells if these
are not originally specified during allocation application. (ie.
specific dependencies on shells MUST be declared and tested in advance,
eg. via the preparatory access track).

The login shells baseline and user selection policy MAY vary;
in that case it MUST be documented at each center’s website or system.

Default Login Shell Baseline Set
* Bourne (sh)
* Korn (ksh)
* C shell (csh)
* Extended C-shell (tcsh)
* GNU Bourne-again shell (bash)
* Z shell (zsh)
