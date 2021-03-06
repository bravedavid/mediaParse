AUTOMAKE_OPTIONS = subdir-objects
ACLOCAL_AMFLAGS = -I m4

AM_CFLAGS = -I. -Wall -std=c99 $(EXTRA_CFLAGS)
AM_LDFLAGS = -lm

bin_PROGRAMS = hevc_analyze 

hevc_analyze_SOURCES = hevc_analyze.c hevc_stream.c h264_stream.c h264_sei.c hevc_nal.c h264_nal.c

include_HEADERS = hevc_stream.h 
pkginclude_HEADERS = hevc_stream.h h264_stream.h h264_sei.h bs.h

clean-local:
	rm -rf *.pc
