INCLUDES = -I$(top_srcdir)/lib/interfaces \
	-I$(top_srcdir)/lib/interfaces/extensions -I$(top_srcdir)/lib/util -I$(top_srcdir)/lib/widgets/propeditor \
	$(all_includes)
METASOURCES = AUTO
lib_LTLIBRARIES = libkdevbuildbase.la
libkdevbuildbase_la_LDFLAGS = $(all_libraries)
libkdevbuildbase_la_LIBADD = $(top_builddir)/lib/interfaces/libkdevinterfaces.la $(LIB_QT) $(LIB_KDEUI)
libkdevbuildbase_la_SOURCES = kdevbuildtool.cpp
kdevelopbuildtoolsincludedir = $(includedir)/kdevelop/buildtools/base
kdevelopbuildtoolsinclude_HEADERS = kdevbuildtool.h

DOXYGEN_REFERENCES = dcop interfaces kdecore kdefx kdeui khtml kmdi kio kjs kparts kutils kdevutil kdevinterfaces kdevextensions
DOXYGEN_PROJECTNAME = KDevelop Buildtool Base Library
DOXYGEN_DOCDIRPREFIX = kdevbt
include ../../../Doxyfile.am
