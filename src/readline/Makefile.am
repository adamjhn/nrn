## The library that we make:
lib_LTLIBRARIES = libreadline.la

libreadline_la_SOURCES = readline.c history.c funmap.c keymaps.c

noinst_HEADERS = chardefs.h emacs_keymap.h history.h keymaps.h \
	readline.h vi_keymap.h

install-exec-hook:
	rm -f $(DESTDIR)$(libdir)/libreadline0@SHREXT@
	$(LN_S) $(DESTDIR)$(libdir)/libreadline@SHREXT@ $(DESTDIR)$(libdir)/libreadline0@SHREXT@
