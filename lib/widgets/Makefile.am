INCLUDES = -I$(top_srcdir)/lib/compat -I$(top_srcdir)/lib/interfaces $(all_includes)

METASOURCES = AUTO

lib_LTLIBRARIES = libkdevwidgets.la

kdevwidgetsincludedir = $(includedir)/kdevelop/widgets

libkdevwidgets_la_SOURCES = flagboxes.cpp qcomboview.cpp klistviewaction.cpp \
	kcomboview.cpp resizablecombo.cpp kdevhtmlpart.cpp processlinemaker.cpp \
	processwidget.cpp ksavealldialog.cpp fancylistviewitem.cpp


kdevwidgetsinclude_HEADERS = klistviewaction.h qcomboview.h flagboxes.h \
	ksavealldialog.h resizablecombo.h kcomboview.h kdevhtmlpart.h processlinemaker.h \
	processwidget.h fancylistviewitem.h 
	

SUBDIRS = propeditor

libkdevwidgets_la_LIBADD = $(top_builddir)/lib/interfaces/libkdevinterfaces.la
libkdevwidgets_la_LDFLAGS = -no-undefined $(all_libraries)
rcdir = $(kde_datadir)/kdevelop

rc_DATA =  kdevhtml_partui.rc

DOXYGEN_REFERENCES = dcop interfaces kdecore kdefx kdeui khtml kmdi kio kjs kparts kutils kdevutil kdevinterfaces
DOXYGEN_PROJECTNAME = KDevelop Widgets Library
DOXYGEN_DOCDIRPREFIX = kdev
include ../../Doxyfile.am
