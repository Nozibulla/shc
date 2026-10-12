bin_PROGRAMS = shc
shc_SOURCES = shc.c


check: shc
	/bin/bash "$(srcdir)/../test/runner.sh"
	/bin/bash "$(srcdir)/../test/filenames.sh" ./shc
	/bin/bash "$(srcdir)/../test/errors.sh" ./shc
	/bin/bash "$(srcdir)/../test/bash-static.sh" ./shc
	/bin/bash "$(srcdir)/../test/output-paths.sh" ./shc
	$(srcdir)/../test/ttest.sh ./shc

