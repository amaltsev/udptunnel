dnl Process this file with autoconf to produce a configure script.
AC_INIT(udptunnel.c)

AM_INIT_AUTOMAKE(udptunnel, 1.1)

dnl Checks for programs.
AC_PROG_CC
AC_PROG_MAKE_SET

if [[ "x$GCC" = "xyes" ]]; then
  CFLAGS="$CFLAGS -Wall"
fi


dnl Checks for libraries.
AC_CHECK_LIB(nsl, gethostname)
AC_CHECK_LIB(socket, socket)

dnl Checks for header files.
AC_HEADER_STDC
AC_CHECK_HEADERS(fcntl.h sys/time.h unistd.h)

dnl Checks for typedefs, structures, and compiler characteristics.
AC_CHECK_SIZEOF(short)

dnl Checks for library functions.
AC_CHECK_FUNCS(select socket strtol)

AC_OUTPUT(Makefile)
