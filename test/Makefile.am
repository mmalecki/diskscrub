check_PROGRAMS = pad trand aestest tprogress tgetsize tsig tsize pat

TESTS_ENVIRONMENT = env 
TESTS_ENVIRONMENT += "PATH_SCRUB=$(top_builddir)/src/scrub"
TESTS = t00 t01 t02 t03 t04 t05 t06 t07 t08 t09 t10 t11 t12 t13 t14
EXPS = t00.exp t01.exp t02.exp t03.exp t04.exp t05.exp t06.exp t07.exp \
	t08.exp t10-cartman.exp t10-jimmy.exp t10-manbearpig.exp \
	t10-marklar.exp t10-timmy.exp t11.exp t12.exp t13.exp t14.exp

CLEANFILES = *.out *.diff testfile

AM_CFLAGS = -I$(top_srcdir)/src

common_sources = \
	$(top_srcdir)/src/getsize.c \
	$(top_srcdir)/src/genrand.c \
	$(top_srcdir)/src/hwrand.c \
	$(top_srcdir)/src/aes.c \
	$(top_srcdir)/src/util.c \
	$(top_srcdir)/src/progress.c \
	$(top_srcdir)/src/sig.c

pad_SOURCES = pad.c $(common_sources)
trand_SOURCES = trand.c $(common_sources)
aestest_SOURCES = aestest.c $(common_sources)
tprogress_SOURCES = tprogress.c $(common_sources)
tgetsize_SOURCES = tgetsize.c $(common_sources)
tsig_SOURCES = tsig.c $(common_sources)
pat_SOURCES = pat.c $(common_sources)

EXTRA_DIST = $(TESTS) $(EXPS)
