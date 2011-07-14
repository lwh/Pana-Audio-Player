kde_module_LTLIBRARIES = libpana_daap-mediadevice.la
kde_services_DATA = pana_daap-mediadevice.desktop

INCLUDES = \
 -I$(top_srcdir)/pana/src \
 -I$(top_builddir)/pana/src/panacore \
 -I$(top_builddir)/pana/src \
 -I$(top_srcdir)/pana/src/panacore \
 -I$(top_srcdir)/pana/src/engine \
 -I$(top_srcdir)/pana/src/engine \
 -I$(top_srcdir)/pana/src/mediadevice \
 $(TAGLIB_CFLAGS) \
 $(all_includes)

METASOURCES = AUTO

libpana_daap_mediadevice_la_LIBADD  = \
 $(top_builddir)/pana/src/libpana.la \
 $(top_builddir)/pana/src/mediadevice/daap/daapreader/libdaapreader.la \
 $(DNSSD_LIBS) ${LIB_KDEUI} ${LIB_KDECORE} ${LIB_KIO}

libpana_daap_mediadevice_la_LDFLAGS = \
 $(KDE_PLUGIN) \
 $(all_libraries)

libpana_daap_mediadevice_la_SOURCES = \
 addhostbase.ui \
 daapclient.cpp \
 daapserver.cpp \
 proxy.cpp

noinst_HEADERS = \
 daapclient.h \
 daapserver.h \
 proxy.h

bin_SCRIPTS = pana_daapserver.rb

SUBDIRS = daapreader mongrel

panarubylibdir = \
  $(kde_datadir)/pana14/ruby_lib

panarubylib_DATA = \
 codes.rb
