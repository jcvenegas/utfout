#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

m4_define([utfout_version], 0.0.2)

AC_PREREQ([2.68])
AC_INIT([utfout], [utfout_version], [jamesodhunt@ubuntu.com])
AC_COPYRIGHT([Copyright (C) 2012-2015 James Hunt <jamesodhunt@ubuntu.com>])

AC_CONFIG_MACRO_DIR([m4])
AC_CONFIG_SRCDIR([src/utfout.c])
AC_CONFIG_HEADERS([config.h])
AC_CONFIG_AUX_DIR([config])

AC_SUBST(UTFOUT_VERSION, utfout_version)

AM_GNU_GETTEXT_VERSION([0.18.1])
AM_GNU_GETTEXT([external])

# Checks for programs.
AC_PROG_CC

# Checks for libraries.

# Checks for header files.
AC_HEADER_STDC
#AC_CHECK_HEADERS([fcntl.h langinfo.h locale.h paths.h stdlib.h string.h unistd.h wchar.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_TYPE_SIZE_T

# Checks for library functions.
AC_CHECK_FUNCS([nl_langinfo setlocale strdup])

AM_INIT_AUTOMAKE
AC_CONFIG_FILES([ Makefile
                 src/Makefile
                 po/Makefile.in
                 utfout.spec ])
AC_OUTPUT
