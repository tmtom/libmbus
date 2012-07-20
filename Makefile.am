#
#
#
PACKAGE		= @PACKAGE@
VERSION		= @VERSION@

pkgconfigdir = $(libdir)/pkgconfig
pkgconfig_DATA = libmbus-@LIBMBUS_API_VERSION@.pc


docdir = $(datadir)/doc/$(PACKAGE)-$(VERSION)
dist_docdir = $(DESTDIR)$(docdir)
doc_DATA = README \
           COPYING \
           hardware/MBus_USB.pdf \
           hardware/MBus_USB.txt

SUBDIRS		= mbus bin
ACLOCAL		= aclocal -I .
ACLOCAL_AMFLAGS = -Werror -I m4
