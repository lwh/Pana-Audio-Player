INCLUDES = \
    -I$(top_builddir)/pana/src \
    -I$(top_builddir)/pana/src/panacore \
    -I$(top_srcdir)/pana/src \
    -I$(top_srcdir)/pana/src/engine \
    -I$(top_srcdir)/pana/src/plugin \
    -I$(top_srcdir)/pana/src/statusbar \
    -I$(top_srcdir)/pana/src/mediadevice \
    $(all_includes)

noinst_LTLIBRARIES = \
    libpanacore.la

noinst_HEADERS = \
    panaconfig.h \
    panadcophandler.h

libpanacore_la_SOURCES = \
    panadcopiface.skel \
    panadcophandler.cpp \
    panaconfig.kcfgc \
    crashhandler.cpp

METASOURCES = \
    AUTO

kde_kcfg_DATA = \
    pana.kcfg
