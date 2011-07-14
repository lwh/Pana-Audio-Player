INCLUDES = -I$(top_srcdir)/pana/src/panacore $(all_includes)
METASOURCES = AUTO

kde_module_LTLIBRARIES = konqsidebar_universalpana.la

konqsidebar_universalpana_la_SOURCES = universalpana.cpp panadcopiface.stub
konqsidebar_universalpana_la_LDFLAGS = -module $(KDE_PLUGIN) $(all_libraries) -lkonqsidebarplugin
konqsidebar_universalpana_la_LIBADD = $(LIB_KHTML) $(LIB_KPARTS) $(LIB_KFILE)


panadcopiface_DIR=$(top_srcdir)/pana/src/panacore
universalpana_add_DATA = pana.desktop
universalpana_adddir = $(kde_datadir)/konqsidebartng/add

universalpana_kickerentries_DATA = pana.desktop
universalpana_kickerentriesdir = $(kde_datadir)/konqsidebartng/kicker_entries

universalpana_entries_DATA = pana.desktop
universalpana_entriesdir = $(kde_datadir)/konqsidebartng/entries

noinst_HEADERS = universalpana.h 
