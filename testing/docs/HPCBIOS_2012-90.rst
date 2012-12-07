.. _HPCBIOS_2012-90:

HPCBIOS_2012-90: Software Development Environment
=================================================

.. note::

  Software Development environment includes a set of tools which are needed
  for building and using scientific computing software.
  The following is an attempt to define which ones are relevant
  for the HPCBIOS communities and set an action plan.

  * BC Policy: HPCBIOS_2012-90
  * Date of Policy: 2012-12-15

The main objective of this policy is to provide the following common
productivity environment across any HPCBIOS resources:

+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| Name                                             | Prefered version(s)   | Compliance level   | Subcategory                                        |
+==================================================+=======================+====================+====================================================+
| bash sh tcsh ksh csh zsh                         | latest                | MUST               | 01. unix shells                                    |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| vim emacs nano joe jove ed sed                   | latest                | SHOULD             | 02. editors / stream editors                       |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| coreutils bc tar grep gawk findutils parallel    | latest                | SHOULD             | 03. GNU variations of common Unix tools            |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| more less screen script                          | latest                | SHOULD             | 04. user interaction                               |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| man help2man texinfo par                         | latest                | SHOULD             | 05. online help                                    |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| zlib openssl openssh                             | latest                | SHOULD             | 06. zlib/openssl are typically required allover    |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| wget lynx links curl rsync unison ftp lftp bbcp  | latest                | SHOULD             | 07. downloaders / file fetchers                    |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| subversion rcs cvs git git-core git-svn          | latest                | SHOULD             | 10. version control                                |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| ssh ldap nfs nscd telnet netcat ntp ntpdate      | latest                | SHOULD             | 11. system interconnection essentials              |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| strace ltrace lsof finger pwgen procps fuser     | latest                | SHOULD             | 12. process & user inspection                      |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| dstat sysstat iotop htop host ifconfig arp       | latest                | SHOULD             | 13. system inspection tools                        |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| nmap tcpdump dig bind-utils whois icmpinfo       | latest                | SHOULD             | 14. network inspection tools                       |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| ping traceroute ping6 traceroute6 tcptrace mtr   | latest                | SHOULD             | 15. network diagnostics - basics                   |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| iperf nuttcp bwctl ndp ndt thrulay               | latest                | SHOULD             | 16. network diagnostics - for IPv6                 |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| patch diff diffstat m4                           | latest                | SHOULD             | 17. patching & macros                              |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| bzip2 zip unzip pax arc lzip rzip cpio           | latest                | SHOULD             | 18. archivers                                      |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| dmidecode lspci blkid fdisk hdparm ethtool       | latest                | SHOULD             | 19. hardware & devices inspection                  |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| make cmake autoconf automake autotools           | latest                | SHOULD             | 20. build tools                                    |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| yasm nasm dev86                                  | latest                | SHOULD             | 21. assembly tools                                 |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| bison byacc flex                                 | latest                | SHOULD             | 22. parsing tools                                  |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| GMP MPFR MPC PPL antlr expect                    | latest                | MUST               | 23. http://gcc.gnu.org/install/prerequisites.html  |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| gcc g++                                          | v4.4.5, v4.6.3        | MUST               | 24. gcc compiler: http://gcc.gnu.org               |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| g77 gfortran libf2c libc6-prof libgfortran3      | latest                | SHOULD             | 25. compiler related                               |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| libtool libltdl-dev ia32-libs                    | latest                | SHOULD             | 26. lib or arch related                            |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| gdb valgrind gprof oprofile time objdump         | latest                | SHOULD             | 27. debugging, profiling, timing                   |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| lsb-release mc                                   | latest                | SHOULD             | 28. misc platform                                  |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| libstdc++ boost-dev                              | 5 or later            | MAY                | 30. base c++ libraries                             |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| ncurses ncurses-dev                              | latest                | SHOULD             | 31. tui development                                |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| binutils-dev libssl-dev libtiff4-dev libsm-dev   | latest                | SHOULD             | 32. devel libs                                     |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| libmysqlclient-dev libpng12-dev libpq-dev        | latest                | SHOULD             | 33. devel libs, part II                            |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| xutils-dev libx11-dev libxt-dev                  | latest                | SHOULD             | 34. devel, X related                               |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| x11proto-xext-dev libxext-dev libqt4-dev         | latest                | SHOULD             | 35. devel, X related, part II                      |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| tk gtk2 QT                                       | latest                | SHOULD             | 36. X related                                      |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| asciidoc doxygen doxygen-doc graphviz            | latest                | SHOULD             | 40. documentation related                          |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| sqlite3 sqlite3-dev                              | latest                | SHOULD             | 50. db                                             |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| python ruby ri perl ipython ocaml tcl            | latest                | SHOULD             | 60. scripting & prototyping                        |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| pychecker pyflakes pylint                        | latest                | SHOULD             | 61. python code checkers                           |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| python-git python-svn                            | latest                | SHOULD             | 62. scripting integration with SCM                 |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| openjdk                                          | v1.6.0                | MAY                | 70. java SDK/Sun JDK                               |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+
| openmpi mpich2 mpich                             | latest                | MAY                | 80. mpi stacks                                     |
+--------------------------------------------------+-----------------------+--------------------+----------------------------------------------------+

This productivity environment will be supplemented with other related
productivity tools as they become available on allocated systems.

Potential sources of information for future upgrades of this list include:
  * http://wiki.gumstix.org/index.php?title=Build_Environment_openSUSE_11.0
  * http://www.grid5000.fr/mediawiki/index.php/FC11_Tlse
  * http://sebastien.dinot.free.fr/liens_dev_c_cpp.html

Kindly notify -if this policy is inadequate for your work-
both your local site technical representative & HPCBIOS user-support.
