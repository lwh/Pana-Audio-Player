kde_module_LTLIBRARIES = libpana_nfs-device.la
kde_services_DATA = pana_nfs-device.desktop

INCLUDES = \
    -I$(top_builddir)/pana/src/panacore \
    -I$(top_srcdir)/pana/src/panacore \
    -I$(top_builddir)/pana/src/panacore \
    -I$(top_srcdir)/pana/src/plugin \
    -I$(top_builddir)/pana/src \
    -I$(top_srcdir)/pana/src \
     $(all_includes)

METASOURCES = AUTO

libpana_nfs_device_la_LIBADD = \
    $(top_builddir)/pana/src/libpana.la \
    -lkdecore

libpana_nfs_device_la_LDFLAGS = \
    $(KDE_PLUGIN) \
    $(all_libraries)







noinst_HEADERS = nfsdevicehandler.h
libpana_nfs_device_la_SOURCES = nfsdevicehandler.cpp
