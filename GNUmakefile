PROJECT=sh-s2b
VERSION=1.0.0
PREFIX=/usr/local
all:
clean:
install:

## -- BLOCK:license --
install: install-license
install-license: 
	install -D -t $(DESTDIR)$(PREFIX)/share/doc/$(PROJECT) LICENSE
## -- BLOCK:license --
## -- BLOCK:sh --
install: install-sh
install-sh:
	mkdir -p $(DESTDIR)$(PREFIX)/bin
	cp bin/s2b              $(DESTDIR)$(PREFIX)/bin
	cp bin/s2b_example      $(DESTDIR)$(PREFIX)/bin
## -- BLOCK:sh --
