kde_module_LTLIBRARIES = \
    libpana_yauap-engine_plugin.la

INCLUDES = \
    -I$(top_srcdir)/pana/src/plugin \
    -I$(top_srcdir)/pana/src \
    $(CFLAGS_YAUAP) \
    $(all_includes)



libpana_yauap_engine_plugin_la_LIBADD = \
    $(top_builddir)/pana/src/libpana.la \
    $(top_builddir)/pana/src/plugin/libplugin.la \
    $(LIB_YAUAP)\
    $(LIB_KDECORE)


libpana_yauap_engine_plugin_la_SOURCES = \
    yauap-engine.cpp

libpana_yauap_engine_plugin_la_LDFLAGS = \
    $(KDE_PLUGIN) \
    $(all_libraries)

METASOURCES = AUTO

kde_services_DATA = \
    pana_yauap-engine_plugin.desktop
