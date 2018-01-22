DB2MAN = docbook-to-man
RM = rm

include_HEADERS = hello.h

lib_LTLIBRARIES = libhello.la
libhello_la_SOURCES = hello.c
man1_MANS = libhello.3

libhello.3: libhello.sgml
	$(DB2MAN) $< >$@

clean-local:
	$(RM) -f $(man3_MANS)
