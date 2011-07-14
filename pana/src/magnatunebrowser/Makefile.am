INCLUDES = -I$(top_builddir)/pana/src/panacore     -I$(top_srcdir)/pana/src/panacore     -I$(top_srcdir)/pana/src/analyzers     -I$(top_srcdir)/pana/src/plugin     -I$(top_srcdir)/pana/src/statusbar     -I$(top_srcdir)/pana/src/mediadevice     -I$(top_srcdir)/pana/src/device     -I$(top_srcdir)/pana/src     -I$(kde_includes)/arts     $(TAGLIB_CFLAGS)     $(sqlite_includes)     $(mysql_includes)     $(postgresql_includes)     $(EXSCALIBAR_CFLAGS)     $(all_includes)
METASOURCES = AUTO


noinst_LTLIBRARIES = libmagnatunebrowser.la
libmagnatunebrowser_la_SOURCES = magnatuneartistinfobox.cpp \
	magnatunebrowser.cpp magnatunedownloaddialogbase.ui magnatunedownloaddialog.cpp \
	magnatunepurchasedialogbase.ui magnatunepurchasedialog.cpp magnatunepurchasehandler.cpp \
	magnatunetypes.cpp magnatunexmlparser.cpp magnatunedatabasehandler.cpp \
	magnatunelistviewitems.cpp magnatunelistview.cpp magnatuneredownloaddialog.cpp \
	magnatuneredownloadhandler.cpp magnatunedownloadinfo.cpp magnatunealbumdownloader.cpp \
	magnatuneredownloaddialogbase.ui
noinst_HEADERS = magnatunedatabasehandler.h magnatunelistviewitems.h \
	magnatunelistview.h magnatuneartistinfobox.h magnatunebrowser.h magnatunedownloaddialog.h \
	magnatunepurchasedialog.h magnatunepurchasehandler.h magnatunetypes.h magnatunexmlparser.h \
	magnatunedownloadinfo.h magnatunealbumdownloader.h
