kde_module_LTLIBRARIES = libpana_masengine_plugin.la
kde_services_DATA = pana_masengine_plugin.desktop

INCLUDES = \
    -I$(top_srcdir)/pana/src/engine \
    -I$(top_srcdir)/pana/src/plugin \
    -I$(top_srcdir)/pana/src \
    $(CFLAGS_MAS) $(all_includes)

libpana_masengine_plugin_la_LIBADD = \
    $(top_builddir)/pana/src/engine/libengine.la \
    $(top_builddir)/pana/src/plugin/libplugin.la \
    $(LIB_KFILE) $(LIB_KDEUI) $(LIB_KDECORE) \
    $(LIBS_MAS)

libpana_masengine_plugin_la_SOURCES = \
    masengine.cpp

libpana_masengine_plugin_la_LDFLAGS = \
    -module \
    -no-undefined \
    $(KDE_PLUGIN) \
    $(all_libraries) 

METASOURCES = AUTO



