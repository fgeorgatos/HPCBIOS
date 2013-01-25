.. _HPCBIOS_06-04:

HPCBIOS_06-04: Baseline Editors and Scripting Tools
===================================================

.. note::
  Each site MUST install and maintain the following baseline set of
  editors and scripting tools. New versions of these packages SHOULD
  be installed within 30 days of their availability on all allocated HPC
  systems and non-storage user-accessible support servers, and they SHOULD
  be installed in the users default path. References for obtaining
  information and downloading these packages are included below.
  Sites MAY choose to provide certain versions via modules framework.

  * BC Policy: HPCBIOS_06-04
  * Date of Policy: 2012-12-15

Baseline shells are covered by policy [HPCBIOS_05-06]

Baseline Editors

+--------------+--------------------------------------------------------+----------+
| Emacs        | http://www.gnu.org/software/emacs/emacs.html           | MUST     |
+--------------+--------------------------------------------------------+----------+
| Vi and Vim   | http://ex-vi.sourceforge.net    http://www.vim.org     | MUST     |
+--------------+--------------------------------------------------------+----------+
| Eclipse      | http://www.eclipse.org                                 | SHOULD   |
+--------------+--------------------------------------------------------+----------+
| Nano         | http://www.nano-editor.org                             | SHOULD   |
+--------------+--------------------------------------------------------+----------+
| Nedit        | http://www.nedit.org                                   | SHOULD   |
+--------------+--------------------------------------------------------+----------+
| Pico         | http://www.washington.edu/pine/                        | SHOULD   |
+--------------+--------------------------------------------------------+----------+
| Joe          | http://freshmeat.net/projects/joe                      | SHOULD   |
+--------------+--------------------------------------------------------+----------+
| Jove         | http://freshmeat.net/projects/jove                     | SHOULD   |
+--------------+--------------------------------------------------------+----------+

Baseline Scripting Tools

+----------+------------------------------+----------+
| Expect   | http://expect.nist.gov       | MUST     |
+----------+------------------------------+----------+
| Perl     | http://www.perl.org          | MUST     |
+----------+------------------------------+----------+
| Java     | http://www.java.com          | SHOULD   |
+----------+------------------------------+----------+
| Ruby     | http://www.ruby-lang.org     | SHOULD   |
+----------+------------------------------+----------+
| PHP      | http://www.php.org           | SHOULD   |
+----------+------------------------------+----------+
| Tcl/Tk   | http://www.tcl.tk            | SHOULD   |
+----------+------------------------------+----------+

.. seealso::
  Python and its scientific add-on components are fully covered in Baseline Configuration
  policy |HPCBIOS_10-02| entitled “Common Open Source High Productivity Languages.”

.. |HPCBIOS_10-02| replace:: [:ref:`HPCBIOS_10-02 <HPCBIOS_10-02>`]

