#                                               -*- Autoconf -*-
# Copyright (C) 2014, Enrico M. Crisostomo <enrico.m.crisostomo@gmail.com>
#
# This program is free software; you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation; either version 3, or (at your option)
# any later version.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with this program.  If not, see <http://www.gnu.org/licenses/>.
#
# Process this file with autoconf to produce a configure script.
dnl Copyright (C) 2014, Enrico M. Crisostomo
AC_PREREQ([2.69])
m4_include([m4/dsc_version.m4])
AC_INIT([dsc], [DSC_VERSION], [enrico.m.crisostomo@gmail.com])
AC_COPYRIGHT([2014 (C) Enrico M. Crisostomo])
AC_REVISION([$Revision: DSC_REVISION$])
AC_CONFIG_SRCDIR([dsc.in])
AC_CONFIG_AUX_DIR([config])
AC_CONFIG_HEADERS([config.h])
AC_CONFIG_FILES([Makefile])
AC_CONFIG_FILES([dsc])
AC_CONFIG_MACRO_DIR([m4])

AM_INIT_AUTOMAKE([-Wall -Werror gnu])

# Checks for programs.
AC_PATH_PROG([zsh], [zsh], [no])
if test x"${ac_cv_path_zsh}" = x"no"
then
  AC_MSG_ERROR([This script requires zsh to run.])
fi
ZSH_PATH=${ac_cv_path_zsh}
AC_SUBST([ZSH_PATH])

AC_PATH_PROG([column], [column], [no])
if test x"${ac_cv_path_column}" = x"no"
then
  AC_MSG_WARN([column not found, some features will be missing.])
  HAVE_COLUMN=0
else
  HAVE_COLUMN=1
fi
COLUMN_PATH=${ac_cv_path_column}
AC_SUBST([COLUMN_PATH])
AC_SUBST([HAVE_COLUMN])

# Checks for libraries.

# Checks for header files.

# Checks for typedefs, structures, and compiler characteristics.

# Checks for library functions.

AC_OUTPUT
