bin_PROGRAMS = shc
shc_SOURCES = shc.c


check: shc
	/bin/bash "$(srcdir)/../test/runner.sh"
	/bin/bash "$(srcdir)/../test/filenames.sh" ./shc
	/bin/bash "$(srcdir)/../test/errors.sh" ./shc
	/bin/bash "$(srcdir)/../test/bash-static.sh" ./shc
	/bin/bash "$(srcdir)/../test/output-paths.sh" ./shc
	CC="$(CC)" CPPFLAGS="$(CPPFLAGS)" CFLAGS="$(CFLAGS)" LDFLAGS="$(LDFLAGS)" /bin/bash "$(srcdir)/../test/arg-max.sh"
	$(srcdir)/../test/ttest.sh ./shc

