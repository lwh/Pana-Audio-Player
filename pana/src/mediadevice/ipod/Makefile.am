kde_module_LTLIBRARIES = libpana_ipod-mediadevice.la
kde_services_DATA = pana_ipod-mediadevice.desktop

INCLUDES = \
    -I$(top_srcdir)/pana/src \
    -I$(top_builddir)/pana/src \
    -I$(top_srcdir)/pana/src/panacore \
    -I$(top_builddir)/pana/src/panacore \
    -I$(top_srcdir)/pana/src/engine \
    -I$(top_builddir)/pana/src/engine \
    -I$(top_srcdir)/pana/src/mediadevice \
    $(LIBGPOD_CFLAGS) \
    $(TAGLIB_CFLAGS) \
    $(all_includes)

METASOURCES = AUTO

libpana_ipod_mediadevice_la_LIBADD  = \
    $(top_builddir)/pana/src/libpana.la

libpana_ipod_mediadevice_la_LDFLAGS = \
    $(KDE_PLUGIN) \
    $(LIBGPOD_LIBS) \
    $(all_libraries)

libpana_ipod_mediadevice_la_SOURCES = \
    ipodmediadevice.cpp

noinst_HEADERS = \
    ipodmediadevice.h

