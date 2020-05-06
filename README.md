# xterm-set-title

Simple script to set the title of the current [XTerm][XTERM-HOME] (or of a
similarly-behaved [terminal emulator][TERMINAL-EMULATOR-WIKIPEDIA]).


# Overview

This is the README.md file for the `'xterm-set-title'` project.

The `xterm-set-title` project provides a simple command line tool that allows
you to easily set the title for your current xterm from the command line.

The 'xterm-set-title' project web site is:

   * https://salewski.github.io/xterm-set-title/

The latest version of the project is `0.1.0` (released 2020-05-06), and can be
downloaded from:

   * https://salewski.github.io/xterm-set-title/downloads/xterm-set-title-0.1.0.tar.gz
   * https://salewski.github.io/xterm-set-title/downloads/xterm-set-title-0.1.0.tar.gz.SHA-1
   * https://salewski.github.io/xterm-set-title/downloads/xterm-set-title-0.1.0.tar.gz.SHA-256
   * https://salewski.github.io/xterm-set-title/downloads/xterm-set-title-0.1.0.tar.gz.SHA3-256

See the [NEWS] file for changes for this release.

Older releases are available from the project's downloads page:

   * https://salewski.github.io/xterm-set-title/downloads/


# Usage

From your shell within an [xterm(1)][XTERM-MAN-1] (or work-alike), do this:

``` sh
    $ xterm-set-title 'My New Title'
```

See the "Prerequisites" section below for other programs that must be
installed and configured on your system before you can install the
`'xterm-set-title'` package.

See the [BUGS] file for information on reporting bugs.

See the [INSTALL] file for installation instructions.

See the [HACKING] file for developer build instructions and the like.

See the [NEWS] file for changes for this release, and a running list of
changes from previous releases. Any incompatibilities with previous versions
will be noted in the `'NEWS'` file.


# Prerequisites

The tool(s) provided by the `'xterm-set-title'` project are intended to be
built and run on Unix and Unix-like systems, so expect a standard set of
utilities (`cat`, `sed`, `awk`, `rm`, ...) to be present. These utilities are
not explicitly listed below as prerequisites as they should be present on any
modern Unix or GNU/Linux system (or in Cygwin, if you happen to be running on
MS Windows).

The `'xterm-set-title'` tool is implemented in [Bash][BASH-HOME]
(a [Bourne shell][BOURNE-YOUTUBE] derivative). The 'xterm-set-title' project
was developed and tested using various versions of Bash at different times,
most recently version 5.0.3(1). It uses associative arrays which
[were added in Bash 4.0][BASH-CHANGES], so you'll need a 4.x version or newer;
the `'configure'` script will check for this and exit with an error message if
a new enough version of Bash is not found. The author would appreciate hearing
about any successes or failures with other versions of Bash. In the unlikely
event that your system does not already have bash installed, it can be
obtained from the project's site:

   * http://www.gnu.org/software/bash/

On a Debian system (including derivatives, such as Ubuntu), you can install
the program via:
```
    # apt-get install bash
```

or (for a statically linked version):
```
    # apt-get install bash-static
```


# See also

   * [xterm(1)][XTERM-MAN-1] man page
   * [XTerm project home page][XTERM-HOME]
   * ["xterm"][XTERM-WIKIPEDIA] (Wikipedia page)


# Disclaimer

While the author of the `xterm-set-title` project is a grateful and long-time
user of the XTerm program, the `xterm-set-title` project is neither affiliated
with the official XTerm development nor endorsed by
[Thomas E. Dickey][T.E.DICKEY-HOME], the current XTerm developer. Any problems
with the `xterm-set-title` program or it's packaging should be reported to
Alan D. Salewski; see the [BUGS] file for guidelines on how to do so.


# License

GPLv2+: GNU GPL version 2 or later <http://gnu.org/licenses/gpl.html>

Unless otherwise stated by a different license notice in a particular file,
all files in the `xterm-set-title' project are made available under the GNU
GPL version 2, or (at your option) any later version.

See the [COPYING] file for the full license.

Copyright (C) 2020 Alan D. Salewski <salewski@att.net>

    This program is free software; you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation; either version 2 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License along
    with this program; if not, write to the Free Software Foundation, Inc.,
    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.


[BUGS]:         https://github.com/salewski/xterm-set-title/blob/master/BUGS     "file: BUGS"
[COPYING]:      https://github.com/salewski/xterm-set-title/blob/master/COPYING  "file: COPYING"
[HACKING]:      https://github.com/salewski/xterm-set-title/blob/master/HACKING  "file: HACKING"
[INSTALL]:      https://github.com/salewski/xterm-set-title/blob/master/INSTALL  "file: INSTALL"
[NEWS]:         https://github.com/salewski/xterm-set-title/blob/master/NEWS     "file: NEWS"

[BASH-HOME]:    https://tiswww.case.edu/php/chet/bash/bashtop.html  "The GNU Bourne-Again Shell"
[BASH-CHANGES]: https://tiswww.case.edu/php/chet/bash/CHANGES       "Bash CHANGES"

[T.E.DICKEY-HOME]:  https://invisible-island.net/    "Thomas E. Dickey's software development projects (invisible-island.net)"

[XTERM-HOME]:   https://invisible-island.net/xterm/  "XTERM – Terminal emulator for the X Window System"

[XTERM-MAN-1]:  https://linux.die.net/man/1/xterm    "xterm(1)"

[XTERM-WIKIPEDIA]:              https://en.wikipedia.org/wiki/Xterm              "xterm (Wikipedia)"
[TERMINAL-EMULATOR-WIKIPEDIA]:  https://en.wikipedia.org/wiki/Terminal_emulator  "Terminal emulator (Wikipedia)"

[BOURNE-YOUTUBE]:  https://www.youtube.com/watch?v=FI_bZhV7wpI  "Early days of Unix and design of sh by Stephen R. Bourne"
