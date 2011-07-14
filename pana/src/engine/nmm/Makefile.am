imagesdir = $(kde_datadir)/pana/images
images_DATA = \
    nmm-gradient-left.png \
    nmm-gradient-right.png \
    nmm-volume-inset.png

kde_module_LTLIBRARIES = \
    libpana_nmmengine_plugin.la

INCLUDES = \
    -I$(top_srcdir)/pana/src \
    $(CFLAGS_NMM) \
    $(all_includes)

libpana_nmmengine_plugin_la_LIBADD = \
    $(top_builddir)/pana/src/libpana.la \
    $(top_builddir)/pana/src/plugin/libplugin.la \
    $(LIB_KDECORE) $(LIB_KFILE) \
    -lnmmbase -lnmmgraphmgr -lnmmiprogress -lnmmiaudiodevice -lnmmigeneral

libpana_nmmengine_plugin_la_SOURCES = \
    nmm_engine.cpp \
    nmm_configdialog.cpp \
    nmm_configdialogbase.ui \
    NmmLocation.cpp \
    HostList.cpp \
    HostListItem.cpp \
    ServerregistryPing.cpp \
    pananmm_kdeconfig.kcfgc

libpana_nmmengine_plugin_la_LDFLAGS = \
    -module \
    $(KDE_PLUGIN) \
    $(LDFLAGS_NMM) \
    $(all_libraries)

METASOURCES = \
    AUTO

KDE_CXXFLAGS = $(USE_EXCEPTIONS)

kde_services_DATA = \
    pana_nmmengine_plugin.desktop

kde_kcfg_DATA = pananmm_kdeconfig.kcfg

SUBDIRS = icons
