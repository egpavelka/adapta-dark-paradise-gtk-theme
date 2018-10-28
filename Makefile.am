ACLOCAL_AMFLAGS = -I m4

themedir  = $/.themes
adaptadir = $(DESTDIR)$(themedir)/adapta-dark-paradise
noktodir  = $(DESTDIR)$(themedir)/adapta-nokto-dark-paradise
adaptaetadir = $(DESTDIR)$(themedir)/adapta-eta-dark-paradise
noktoetadir  = $(DESTDIR)$(themedir)/adapta-nokto-eta-dark-paradise

SUBDIRS = \
	gtk \
	shell \
	wm \
	extra

EXTRA_DIST = \
	COPYING \
	LICENSE_CC_BY_SA4 \
	README.md

install-data-hook:
	cp -Rv $(EXTRA_DIST) $(adaptadir)

uninstall-hook:
	test -e $(noktodir) && rm -rfv $(noktodir)
	test -e $(adaptadir) && rm -rfv $(adaptadir)
	test -e $(noktetaodir) && rm -rfv $(noktoetadir)
	test -e $(adaptaetadir) && rm -rfv $(adaptaetadir)
