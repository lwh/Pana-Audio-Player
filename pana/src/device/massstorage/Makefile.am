kde_module_LTLIBRARIES = libpana_massstorage-device.la
kde_services_DATA = pana_massstorage-device.desktop

INCLUDES = \
    -I$(top_builddir)/pana/src/panacore \
    -I$(top_srcdir)/pana/src/panacore \
    -I$(top_builddir)/pana/src/panacore \
    -I$(top_srcdir)/pana/src/plugin \
    -I$(top_builddir)/pana/src \
    -I$(top_srcdir)/pana/src \
     $(all_includes)

METASOURCES = AUTO

libpana_massstorage_device_la_LIBADD = \
    $(top_builddir)/pana/src/libpana.la \
    -lkdecore

libpana_massstorage_device_la_LDFLAGS = \
    $(KDE_PLUGIN) \
    $(all_libraries)

libpana_massstorage_device_la_SOURCES = \
    massstoragedevicehandler.cpp

noinst_HEADERS = \
    massstoragedevicehandler.h

