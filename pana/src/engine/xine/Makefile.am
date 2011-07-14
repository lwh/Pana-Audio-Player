kde_module_LTLIBRARIES = libpana_xine-engine.la
kde_services_DATA = pana_xine-engine.desktop

INCLUDES = \
    -I$(top_srcdir)/pana/src \
    -I$(top_srcdir)/pana/src/panacore \
    -I$(top_builddir)/pana/src/panacore \
    $(XINE_CFLAGS) \
    $(all_includes)

libpana_xine_engine_la_LIBADD = \
    $(top_builddir)/pana/src/libpana.la \
    $(top_builddir)/pana/src/plugin/libplugin.la \
    -lkdeui -lkdecore \
    $(XINE_LIBS)

libpana_xine_engine_la_SOURCES = \
    xine-scope.c \
    panaxinecfg.kcfgc \
    xine-engine.cpp \
    xineconfigbase.ui \
    xine-config.cpp

libpana_xine_engine_la_LDFLAGS = \
    $(KDE_PLUGIN) \
    $(all_libraries)

kde_kcfg_DATA = \
    panaxinecfg.kcfg

METASOURCES  = AUTO
