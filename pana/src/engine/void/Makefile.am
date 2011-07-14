kde_module_LTLIBRARIES = \
    libpana_void-engine_plugin.la

INCLUDES = \
    -I$(top_srcdir)/pana/src/plugin \
    -I$(top_srcdir)/pana/src \
    $(all_includes)

libpana_void_engine_plugin_la_LIBADD = \
    $(top_builddir)/pana/src/libpana.la \
    $(top_builddir)/pana/src/plugin/libplugin.la \
    $(LIB_KDECORE)

libpana_void_engine_plugin_la_SOURCES = \
    void-engine.cpp

libpana_void_engine_plugin_la_LDFLAGS = \
    $(KDE_PLUGIN) \
    $(all_libraries)

METASOURCES = \
    AUTO

kde_services_DATA = \
    pana_void-engine_plugin.desktop
