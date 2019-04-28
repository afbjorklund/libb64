bin_PROGRAMS = b64

b64_SOURCES = base64.cc

# a larger size should be faster, but takes more runtime memory
#BUFFERSIZE = 4096
#BUFFERSIZE = 65536
BUFFERSIZE=16777216

# rename program to b64, to avoid name conflict with standard base64 from GNU coreutils
AM_CPPFLAGS = -I$(top_srcdir)/include -DPROGRAM_NAME=\"b64\" -DBUFFERSIZE=$(BUFFERSIZE)

LDADD = ../src/libb64.a
