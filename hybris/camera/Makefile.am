lib_LTLIBRARIES = \
	libcamera.la

libcamera_la_SOURCES = camera.c
libcamera_la_CFLAGS = -I$(top_srcdir)/include
if WANT_TRACE
libcamera_la_CFLAGS += -DDEBUG
endif
if WANT_DEBUG
libcamera_la_CFLAGS += -ggdb -O0
endif
libcamera_la_LDFLAGS = \
	$(top_builddir)/common/libhybris-common.la \
	-version-info "1":"0":"0"
