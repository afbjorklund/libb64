bin_PROGRAMS = base64

base64_SOURCES = base64.cc

# a larger size should be faster, but takes more runtime memory
#BUFFERSIZE = 4096
#BUFFERSIZE = 65536
BUFFERSIZE=16777216

AM_CPPFLAGS = -I$(top_srcdir)/include -DBUFFERSIZE=$(BUFFERSIZE)

LDADD = ../src/libb64.a
