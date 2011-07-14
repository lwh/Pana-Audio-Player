kde_module_LTLIBRARIES = libpana_smb-device.la
kde_services_DATA = pana_smb-device.desktop

INCLUDES = \
    -I$(top_builddir)/pana/src/panacore \
    -I$(top_srcdir)/pana/src/panacore \
    -I$(top_builddir)/pana/src/panacore \
    -I$(top_srcdir)/pana/src/plugin \
    -I$(top_builddir)/pana/src \
    -I$(top_srcdir)/pana/src \
     $(all_includes)

METASOURCES = AUTO

libpana_smb_device_la_LIBADD = \
    $(top_builddir)/pana/src/libpana.la \
    -lkdecore

libpana_smb_device_la_LDFLAGS = \
    $(KDE_PLUGIN) \
    $(all_libraries)

noinst_HEADERS = smbdevicehandler.h
libpana_smb_device_la_SOURCES = smbdevicehandler.cpp
