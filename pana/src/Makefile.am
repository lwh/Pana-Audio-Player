if with_included_sqlite
    SQLITE_SUBDIR = sqlite
    LIB_SQLITE_LOCAL = $(top_builddir)/pana/src/sqlite/libsqlite.la
    sqlite_includes = -I$(top_srcdir)/pana/src/sqlite
endif

if with_konqsidebar
    KONQSIDEBAR_SUBDIR = konquisidebar
endif


lib_LTLIBRARIES = libpana.la

SUBDIRS = \
    panacore \
    magnatunebrowser \
    $(SQLITE_SUBDIR) \
    analyzers \
    data \
    plugin \
    images \
    loader \
    scripts \
    themes \
    vis \
    metadata \
    $(KONQSIDEBAR_SUBDIR) \
    statusbar \
    . \
    engine \
    mediadevice \
    device \
    collectionscanner


INCLUDES = \
    -I$(top_builddir)/pana/src/panacore \
    -I$(top_builddir)/pana/src/magnatunebrowser \
    -I$(top_srcdir)/pana/src/panacore \
    -I$(top_srcdir)/pana/src/analyzers \
    -I$(top_srcdir)/pana/src/plugin \
    -I$(top_srcdir)/pana/src/statusbar \
    -I$(top_srcdir)/pana/src/mediadevice \
    -I$(top_srcdir)/pana/src/device \
    -I$(top_srcdir)/pana/src \
    -I$(kde_includes)/arts \
    $(TAGLIB_CFLAGS) \
    $(sqlite_includes) \
    $(mysql_includes) \
    $(postgresql_includes) \
    $(EXSCALIBAR_CFLAGS) \
    $(all_includes)

libpana_la_SOURCES = \
    Options1.ui \
    Options1.ui.h \
    Options2.ui \
    Options4.ui \
    Options5.ui \
    Options7.ui \
    Options8.ui \
    actionclasses.cpp \
    app.cpp \
    atomicstring.cpp \
    atomicurl.cpp \
    browserbar.cpp \
    clicklineedit.cpp \
    collectionbrowser.cpp \
    collectiondb.cpp \
    columnlist.cpp \
    configdialog.cpp \
    contextbrowser.cpp \
    coverfetcher.cpp \
    covermanager.cpp \
    cuefile.cpp \
    dbsetup.ui  \
    dbsetup.ui.h \
    deletedialog.cpp \
    deletedialogbase.ui \
    deviceconfiguredialog.cpp \
    devicemanager.cpp \
    directorylist.cpp \
    dynamicmode.cpp \
    enginebase.cpp \
    enginecontroller.cpp \
    engineobserver.cpp \
    equalizergraph.cpp \
    equalizerpresetmanager.cpp \
    equalizersetup.cpp \
    expression.cpp \
    fht.cpp \
    filebrowser.cpp \
    firstrunwizard.ui \
    hintlineedit.cpp \
    htmlview.cpp \
    iconloader.cpp \
    k3bexporter.cpp \
    kbookmarkhandler.cpp \
    ktrm.cpp \
    lastfm.cpp \
    mediabrowser.cpp \
    mediadevicemanager.cpp \
    medium.cpp \
    mediumpluginmanager.cpp \
    metabundle.cpp \
    metabundlesaver.cpp \
    moodbar.cpp \
    mountpointmanager.cpp \
    multitabbar.cpp \
    mydiroperator.cpp \
    newdynamic.ui \
    organizecollectiondialog.ui \
    osd.cpp \
    pixmapviewer.cpp \
    playerwindow.cpp \
    playlist.cpp \
    playlistbrowser.cpp \
    playlistbrowseritem.cpp \
    playlistitem.cpp \
    playlistloader.cpp \
    playlistselection.cpp \
    playlistwindow.cpp \
    pluginmanager.cpp \
    podcastsettings.cpp \
    podcastsettingsbase.ui \
    prettypopupmenu.cpp \
    queuemanager.cpp \
    scancontroller.cpp \
    scriptmanager.cpp \
    scriptmanagerbase.ui \
    scrobbler.cpp \
    sliderwidget.cpp \
    smartplaylisteditor.cpp \
    socketserver.cpp \
	starmanager.cpp \
    statistics.cpp \
    systray.cpp \
    tagdialog.cpp \
    tagdialogbase.ui \
    tagguesser.cpp \
    tagguesserconfigdialog.ui \
    threadmanager.cpp \
    tooltip.cpp \
    trackpickerdialog.cpp \
    trackpickerdialogbase.ui \
    tracktooltip.cpp \
    transferdialog.cpp \
    xmlloader.cpp \
    xspfplaylist.cpp \
    editfilterdialog.cpp

libpana_la_LIBADD = \
    $(top_builddir)/pana/src/panacore/libpanacore.la \
    $(top_builddir)/pana/src/analyzers/libanalyzers.la \
    $(top_builddir)/pana/src/plugin/libplugin.la \
    $(top_builddir)/pana/src/statusbar/libstatusbar.la \
    $(top_builddir)/pana/src/metadata/libmetadata.la \
    $(top_builddir)/pana/src/magnatunebrowser/libmagnatunebrowser.la \
    $(LIB_KUTILS) $(LIB_KFILE) $(LIB_KDEUI) $(LIB_KDECORE) $(LIB_KHTML) $(LIB_KNEWSTUFF) \
    $(TAGLIB_LIBS) $(gl_libs) $(LIB_SQLITE) $(LIB_SQLITE_LOCAL) \
    $(LIB_TUNEPIMP) \
    $(mysql_libs) \
    $(postgresql_libs)

libpana_la_LDFLAGS = \
    $(all_libraries) \
    $(KDE_RPATH)

METASOURCES = \
    AUTO

KDE_ICON = \
    AUTO



bin_SCRIPTS = pana_proxy.rb

bin_PROGRAMS = panaapp
# atomicstring_unittest is excluded from the build by default to avoid compile slowdowns.
# If you intend to do work in this area and want to build it, comment the line above and
# uncomment the lines below:
#bin_PROGRAMS = panaapp atomicstring_unittest
#atomicstring_unittest_SOURCES = atomicstring_unittest.cpp atomicstring.h
#atomicstring_unittest_LDADD = atomicstring.$(OBJEXT) $(LIB_KDECORE)


panaapp_SOURCES = main.cpp

panaapp_LDADD = \
    $(top_builddir)/pana/src/panacore/libpanacore.la \
    libpana.la \
    $(top_builddir)/pana/src/analyzers/libanalyzers.la \
    $(top_builddir)/pana/src/plugin/libplugin.la \
    $(top_builddir)/pana/src/statusbar/libstatusbar.la \
    $(top_builddir)/pana/src/metadata/libmetadata.la \
    $(LIB_KUTILS) $(LIB_KFILE) $(LIB_KDEUI) $(LIB_KDECORE) $(LIB_KHTML) $(LIB_KNEWSTUFF) \
    $(TAGLIB_LIBS) $(gl_libs) $(LIB_SQLITE) $(LIB_SQLITE_LOCAL) $(EXSCALIBAR_LIBS) \
    $(LIB_TUNEPIMP) \
    $(mysql_libs) \
    $(postgresql_libs)

panaapp_LDFLAGS = \
    $(all_libraries) \
    $(KDE_RPATH)

rcdir = \
    $(kde_datadir)/pana

rc_DATA = \
    panaui.rc


configdir = \
    $(kde_confdir)

config_DATA = \
    panarc


xdg_apps_DATA = \
    pana.desktop

kde_servicetypes_DATA = \
    pana_plugin.desktop \
    pana_codecinstall.desktop


servicemenudir = \
    $(kde_datadir)/konqueror/servicemenus

servicemenu_DATA = \
    pana_addaspodcast.desktop \
    pana_append.desktop \
    pana_play_audiocd.desktop


profiledatadir = \
    $(kde_datadir)/profiles

profiledata_DATA = \
    pana.profile.xml

protocoldir = \
    $(kde_servicesdir)

protocol_DATA = \
    panaitpc.protocol \
    panalastfm.protocol \
    panapcast.protocol

messages: rc.cpp
	$(EXTRACTRC) `find . -name "*.rc" -o -name "*.ui" -o -name "*.kcfg"` > rc.cpp
	LIST=`find . -name \*.h -o -name \*.hh -o -name \*.H -o -name \*.hxx -o -name \*.hpp -o -name \*.cpp -o -name \*.cc -o -name \*.cxx -o -name \*.ecpp -o -name \*.C`; \
	if test -n "$$LIST"; then \
		$(XGETTEXT) $$LIST -o $(podir)/pana.pot; \
	fi

install-exec-hook:
	@echo ""
	@echo "=========================="
	@echo "=  Pana - INSTALLED  ================================"
	@echo "=========================="
	@echo "="
	@echo "=  Type pana to start!"
	@echo "="
	@echo "=  If you have problems, please consult the README;"
	@echo "=  if the problems continue join us on #pana."
	@echo "="
	@echo "======================================================="



