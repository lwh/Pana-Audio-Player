kde_module_LTLIBRARIES = libpana_aKode-engine.la
kde_services_DATA = pana_aKode-engine.desktop

INCLUDES = -I$(top_srcdir)/pana/src $(CFLAGS_AKODE) $(all_includes)

libpana_aKode_engine_la_LIBADD = \
    $(top_builddir)/pana/src/libpana.la \
    $(top_builddir)/pana/src/plugin/libplugin.la \
    -lkdecore \
    $(LIBS_AKODE)

libpana_aKode_engine_la_SOURCES = akode-engine.cpp akode-scope.cpp
libpana_aKode_engine_la_LDFLAGS = -module $(KDE_PLUGIN) $(all_libraries)

METASOURCES  = AUTO
