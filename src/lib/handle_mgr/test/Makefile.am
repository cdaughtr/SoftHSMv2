MAINTAINERCLEANFILES = 		$(srcdir)/Makefile.in

AM_CPPFLAGS = 			-I$(srcdir)/.. \
				-I$(srcdir)/../.. \
				-I$(srcdir)/../../common \
				-I$(srcdir)/../../cryptoki_compat \
				-I$(srcdir)/../../crypto \
				-I$(srcdir)/../../object_store \
				-I$(srcdir)/../../session_mgr \
				-I$(srcdir)/../../slot_mgr \
				-I$(srcdir)/../../data_mgr

AM_CFLAGS =			@CPPUNIT_CFLAGS@

check_PROGRAMS =		handlemgrtest

handlemgrtest_SOURCES =		handlemgrtest.cpp \
				HandleManagerTests.cpp

handlemgrtest_LDADD =		../../libsofthsm_convarch.la 

handlemgrtest_LDFLAGS = 	@CRYPTO_LIBS@ @CPPUNIT_LIBS@ -no-install

TESTS = 			handlemgrtest

EXTRA_DIST =			$(srcdir)/*.h

