SUBDIRS = . tests
if MAKE_DOC
SUBDIRS += doc
endif

lib_LTLIBRARIES = %reldir%/librtmidi.la
%C%_librtmidi_la_LDFLAGS = -no-undefined -export-dynamic -version-info @SO_VERSION@
%C%_librtmidi_la_SOURCES = \
  %reldir%/RtMidi.cpp \
  %reldir%/rtmidi_c.cpp

rtmidi_incdir = $(includedir)/rtmidi
rtmidi_inc_HEADERS = \
  %reldirD%/RtMidi.h \
  %reldirD%/rtmidi_c.h

pkgconfigdatadir = $(libdir)/pkgconfig
pkgconfigdata_DATA = rtmidi.pc

EXTRA_DIST = autogen.sh readme msw

