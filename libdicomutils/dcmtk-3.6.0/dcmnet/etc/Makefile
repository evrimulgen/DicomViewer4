#
#	Makefile for dcmnet/etc
#



SHELL = /bin/sh
srcdir = .
top_srcdir = ..
configdir = ../../config

include $(configdir)/Makefile.def

files = storescp.cfg storescu.cfg


all:

install:
	$(configdir)/mkinstalldirs $(DESTDIR)$(etcdir)
	for file in $(files); do \
		$(INSTALL_DATA) $$file $(DESTDIR)$(etcdir) ;\
	done

clean:
	rm -f $(TRASH)

distclean:
	rm -f $(DISTTRASH)
