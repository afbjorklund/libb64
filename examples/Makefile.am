noinst_PROGRAMS = c-example1 c-example2

c_example1_SOURCES = c-example1.c
c_example2_SOURCES = c-example2.c

AM_CPPFLAGS = -I$(top_srcdir)/include

LDADD = ../src/libb64.a

DEBRIS = encoded.txt decoded.txt

EXTRA_DIST = loremgibson.txt

check-local: check-c-example1 check-c-example2

check-c-example1: c-example1
	./c-example1

check-c-example2: c-example2
	./c-example2 $(srcdir)/loremgibson.txt encoded.txt decoded.txt
	diff -q $(srcdir)/loremgibson.txt decoded.txt

clean-local:
	-$(RM) $(DEBRIS)
