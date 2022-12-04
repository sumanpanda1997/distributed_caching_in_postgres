#-------------------------------------------------------------------------
#
# Makefile--
#    Makefile for tcop
#
# IDENTIFICATION
#    src/backend/tcop/Makefile
#
#-------------------------------------------------------------------------

subdir = src/backend/tcop
top_builddir = ../../..
include $(top_builddir)/src/Makefile.global

OBJS = \
	cmdtag.o \
	dest.o \
	fastpath.o \
	postgres.o \
	pquery.o \
	utility.o

include $(top_srcdir)/src/backend/common.mk

#CS631 start

PG_CPPFLAGS = -I$(libpq_srcdir)
SHLIB_LINK_INTERNAL = $(libpq)
SHLIB_PREREQS = submake-libpq



NO_PGXS = 1
include $(top_srcdir)/src/makefiles/pgxs.mk

#CS631 end
