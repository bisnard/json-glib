include $(top_srcdir)/build/autotools/Makefile.am.gtest
include $(top_srcdir)/build/autotools/Makefile.am.silent

NULL =

DISTCLEANFILES =

INCLUDES = \
	-I$(top_srcdir)			\
	-I$(top_srcdir)/json-glib	\
	$(NULL)

AM_CPPFLAGS = $(JSON_DEBUG_CFLAGS) -DTESTS_DATA_DIR=\""$(top_srcdir)/json-glib/tests"\"
AM_CFLAGS = -g $(JSON_CFLAGS) $(MAINTAINER_CFLAGS)
LDADD = \
	../libjson-glib-1.0.la \
	$(JSON_LIBS) \
	$(NULL)

EXTRA_DIST += stream-load.json

noinst_PROGRAMS = $(TEST_PROGS)
TEST_PROGS += \
	array			\
	boxed			\
	builder			\
	generator		\
	gvariant		\
	invalid			\
	node			\
	object			\
	parser			\
	path			\
	reader			\
	serialize-simple	\
	serialize-complex	\
	serialize-full		\
	$(NULL)

-include $(top_srcdir)/build/autotools/Makefile.am.gitignore
