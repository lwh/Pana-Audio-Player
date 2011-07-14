kde_module_LTLIBRARIES = libpana_generic-mediadevice.la
kde_services_DATA = pana_generic-mediadevice.desktop

INCLUDES = \
    -I$(top_srcdir)/pana/src \
    -I$(top_srcdir)/pana/src/panacore \
    -I$(top_builddir)/pana/src/panacore \
    -I$(top_srcdir)/pana/src/engine \
    -I$(top_srcdir)/pana/src/engine \
    -I$(top_srcdir)/pana/src/mediadevice \
    $(TAGLIB_CFLAGS) \
    $(all_includes)

METASOURCES = AUTO

libpana_generic_mediadevice_la_LIBADD  = \
    $(top_builddir)/pana/src/libpana.la \
    -lkdeui -lkdecore -lkio

libpana_generic_mediadevice_la_LDFLAGS = \
    $(KDE_PLUGIN) \
    $(all_libraries)

libpana_generic_mediadevice_la_SOURCES = \
    genericmediadeviceconfigdialog.ui\
    genericmediadevice.cpp

noinst_HEADERS = \
    genericmediadeviceconfigdialog.ui.h\
    genericmediadevice.h

