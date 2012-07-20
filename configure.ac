dnl ----------------------------------------------------------------------------
dnl Copyright (C) 2010, Raditex AB
dnl All rights reserved.
dnl
dnl rSCADA 
dnl http://www.rSCADA.se
dnl info@rscada.se
dnl 
dnl ----------------------------------------------------------------------------

# Below is a project/package version
AC_INIT([libmbus], [0.8.0], [info@rscada.se], [libmbus], [http://www.rscada.se/libmbus/])
AM_INIT_AUTOMAKE([-Wall -Werror foreign])

AC_CONFIG_MACRO_DIR([m4])
AC_PROG_CC
AM_PROG_LIBTOOL


# Define these substitions here to keep all version information in one place.
# For information on how to properly maintain the library version information,
# refer to the libtool manual, section "Updating library version information":
# http://www.gnu.org/software/libtool/manual/html_node/Updating-version-info.html 

# This is a library/API version in libtool format "current:revision:age"
AC_SUBST([LIBMBUS_SO_VERSION], [0:8:0])
AC_SUBST([LIBMBUS_API_VERSION], [1.0]) 

#LIBMBUS_LIBRARY_VERSION=0:8:0

#LDFLAGS="$LDFLAGS -version-info 0:8:0"

dnl ----------------------
dnl 
AC_PROG_CC

AC_CONFIG_HEADERS([config.h])
AC_CONFIG_FILES([Makefile 
                 mbus/Makefile
                 test/Makefile
                 bin/Makefile
                 libmbus-${LIBMBUS_API_VERSION}.pc:libmbus.pc.in])
AC_OUTPUT


echo \
"----------------------------------------------------------
Configuration:

	Source location:	${srcdir}
	Compile:		${CC}
	Compiler flags:		${CFLAGS}
	Linker flags:		${LDFLAGS}
	Host system type:	${host}
	Install path:		${prefix}

	See config.h for further configuration.
----------------------------------------------------------"
