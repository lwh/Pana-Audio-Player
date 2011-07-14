kde_module_LTLIBRARIES = libpana_mtp-mediadevice.la
kde_services_DATA = pana_mtp-mediadevice.desktop

INCLUDES = \
    -I$(top_srcdir)/pana/src \
    -I$(top_builddir)/pana/src \
    -I$(top_srcdir)/pana/src/panacore \
    -I$(top_builddir)/pana/src/panacore \
    -I$(top_srcdir)/pana/src/engine \
    -I$(top_builddir)/pana/src/engine \
    -I$(top_srcdir)/pana/src/mediadevice \
    $(TAGLIB_CFLAGS) \
    $(all_includes)

METASOURCES = AUTO

libpana_mtp_mediadevice_la_LIBADD  = \
    $(top_builddir)/pana/src/libpana.la \
    $(LIBMTP_LIBS) 

libpana_mtp_mediadevice_la_LDFLAGS = \
    $(KDE_PLUGIN) \
    $(all_libraries)

libpana_mtp_mediadevice_la_SOURCES = \
    mtpmediadevice.cpp

noinst_HEADERS = \
    mtpmediadevice.h

