SUBDIRS = src etc doc

fix-rights:
	$(MAKE) -C src $@

ACLOCAL_AMFLAGS = -I m4

DISTCHECK_CONFIGURE_FLAGS = \
	--with-systemdsystemunitdir=$$dc_install_base/$(systemdsystemunitdir)

EXTRA_DIST = \
	GPL-3.0.txt \
	bootstrap \
	ChangeLog.git \
	DRIVERS SECURITY \
	HELP \
	m4/ax_pthread.m4 \
	m4/as-ac-expand.m4

DISTCLEANFILES = ChangeLog.git

ChangeLog.git:
	git log --stat --decorate=short > $@

