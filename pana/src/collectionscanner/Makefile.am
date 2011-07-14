bin_PROGRAMS = panacollectionscanner

METASOURCES = AUTO

INCLUDES = \
    -I$(top_srcdir)/pana/src \
    $(TAGLIB_CFLAGS) \
    $(all_includes)

noinst_HEADERS = \
    collectionscannerdcophandler.h

panacollectionscanner_SOURCES = \
    main.cpp \
    collectionscannerdcopiface.skel \
    collectionscannerdcophandler.cpp \
    collectionscanner.cpp

panacollectionscanner_LDADD = \
    $(top_builddir)/pana/src/metadata/libmetadata.la \
    $(top_builddir)/pana/src/libpana.la \
    $(LIB_QT) \
    $(LIB_KDECORE) \
    $(TAGLIB_LIBS)

panacollectionscanner_LDFLAGS = \
    $(all_libraries) \
    $(KDE_RPATH)
