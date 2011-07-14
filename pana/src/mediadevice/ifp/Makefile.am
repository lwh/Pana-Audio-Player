kde_module_LTLIBRARIES = libpana_ifp-mediadevice.la
kde_services_DATA = pana_ifp-mediadevice.desktop

INCLUDES = \
    -I$(top_srcdir)/pana/src \
    -I$(top_srcdir)/pana/src/panacore \
    -I$(top_srcdir)/pana/src/statusbar \
    -I$(top_srcdir)/pana/src/engine \
    -I$(top_srcdir)/pana/src/plugin \
    -I$(top_srcdir)/pana/src/mediadevice \
    $(IFP_CFLAGS) \
    $(TAGLIB_CFLAGS) \
    $(all_includes)

libpana_ifp_mediadevice_la_LIBADD = \
    $(top_builddir)/pana/src/libpana.la \
    -lusb -lifp \
    -lkdeui -lkdecore -lkio

libpana_ifp_mediadevice_la_LDFLAGS = \
    $(KDE_PLUGIN) \
    $(all_libraries)

libpana_ifp_mediadevice_la_SOURCES = \
    ifpmediadevice.cpp

METASOURCES = AUTO
