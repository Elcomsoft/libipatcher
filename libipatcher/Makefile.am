AM_CFLAGS = -I$(top_srcdir)/include -I$(top_srcdir)/external/jssy/jssy/ $(GLOBAL_CFLAGS) $(libimg4tool_CFLAGS) $(libimg3tool_CFLAGS) $(libpatchfinder_CFLAGS) $(libgeneral_CFLAGS) $(libfragmentzip_CFLAGS)
AM_LDFLAGS = -L$(top_srcdir)/libipatcher $(GLOBAL_LDFLAGS) $(libimg4tool_LIBS) $(libimg3tool_LIBS) $(libpatchfinder_LIBS) $(libgeneral_LIBS) $(libfragmentzip_LIBS)

noinst_LTLIBRARIES = libjssy.la

lib_LTLIBRARIES = libipatcher.la

libjssy_la_CFLAGS = $(AM_CFLAGS)
libjssy_la_SOURCES = $(top_srcdir)/external/jssy/jssy/jssy.c

libipatcher_la_CXXFLAGS = $(AM_CFLAGS)
libipatcher_la_LIBADD = libjssy.la $(AM_LDFLAGS)
libipatcher_la_SOURCES = libipatcher.cpp
