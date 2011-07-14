kde_services_DATA = pana_njb-mediadevice.desktop


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
kde_module_LTLIBRARIES = libpana_njb-mediadevice.la

libpana_njb_mediadevice_la_LIBADD = $(top_builddir)/pana/src/libpana.la \
	-lkdeui -lkdecore -lnjb

libpana_njb_mediadevice_la_LDFLAGS = $(KDE_PLUGIN) $(all_libraries)

noinst_HEADERS = njbmediadevice.h playlist.h track.h

libpana_njb_mediadevice_la_SOURCES = njbmediadevice.cpp playlist.cpp \
	track.cpp
