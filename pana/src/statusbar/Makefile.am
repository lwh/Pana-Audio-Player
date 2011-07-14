noinst_LTLIBRARIES = libstatusbar.la

METASOURCES = AUTO

INCLUDES = \
    -I$(top_srcdir)/pana/src/ \
    -I$(top_builddir)/pana/src/panacore \
    -I$(top_srcdir)/pana/src/panacore \
    -I$(top_srcdir)/pana/src/engine \
    -I$(top_builddir)/pana/src/ \
    $(all_includes)
    
libstatusbar_la_LIBADD = $(LIB_QT)

libstatusbar_la_SOURCES = \
    statusBarBase.cpp \
    statusbar.cpp \
    overlayWidget.cpp \
    popupMessage.cpp \
    progressBar.cpp \
    squeezedtextlabel.cpp \
    queueLabel.cpp
