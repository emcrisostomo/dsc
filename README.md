README
======

`dsc` is a UNIX shell script that checks the usage percentage of mounted disks
and notifies the user if any of them is above the specified threshold.
Notifications are written by default on the standard output and, optionally,
can be sent by email.

Getting dsc
-----------

The recommended way to install `dsc` in a machine is getting a
[release tarball][release].  A release tarball contains everything a user needs
to build and install this software on a system, following the instructions
detailed in the Installation section below and the INSTALL file.

Getting a copy of the source repository is not recommended, unless you are a
developer, you have the GNU Build System installed on your machine and you know
how to boostrap it on the sources.

[release]: https://github.com/emcrisostomo/dsc/releases

Installation
------------

See the `INSTALL` file for detailed information about how to configure and
install this software.

Dependencies
------------

`dsc` depends on the following programs:

  * The Z Shell (`zsh`).
  * The `mail` local mail transfer agent (MTA).
  * The `df` command.
  * The `column` command (optional).

All mandatory dependencies must be present when running `configure`.  If any
dependency is missing, `configure` will fail and emit a meaningful error
message.

Bug Reports
-----------

Bug reports can be sent directly to the authors.

-----

Copyright (C) 2014, Enrico M. Crisostomo <enrico.m.crisostomo@gmail.com>

This program is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation; either version 3, or (at your option)
any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.
