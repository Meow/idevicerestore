AM_CFLAGS = \
	$(GLOBAL_CFLAGS) \
	$(LFS_CFLAGS) \
	$(libirecovery_CFLAGS) \
	$(libimobiledevice_CFLAGS) \
	$(libusbmuxd_CFLAGS) \
	$(libplist_CFLAGS) \
	$(limd_glue_CFLAGS) \
	$(libzip_CFLAGS) \
	$(zlib_CFLAGS) \
	$(openssl_CFLAGS) \
	$(libcurl_CFLAGS)

AM_LDFLAGS = \
	$(AC_LDFLAGS) \
	$(libirecovery_LIBS) \
	$(libimobiledevice_LIBS) \
	$(libusbmuxd_LIBS) \
	$(libplist_LIBS) \
	$(limd_glue_LIBS) \
	$(libzip_LIBS) \
	$(zlib_LIBS) \
	$(openssl_LIBS) \
	$(libcurl_LIBS)

AM_LDADD = $(AC_LDADD)

bin_PROGRAMS = idevicerestore

idevicerestore_SOURCES = \
	idevicerestore.c idevicerestore.h \
	endianness.h \
	common.c common.h \
	tss.c tss.h \
	fls.c fls.h \
	mbn.c mbn.h \
	img3.c img3.h \
	img4.c img4.h \
	ftab.c ftab.h \
	ipsw.c ipsw.h \
	normal.c normal.h \
	dfu.c dfu.h \
	recovery.c recovery.h \
	restore.c restore.h \
	asr.c asr.h \
	fdr.c fdr.h \
	limera1n_payload.h \
	limera1n.c limera1n.h \
	download.c download.h \
	locking.c locking.h
if USE_INTERNAL_SHA
idevicerestore_SOURCES += sha1.c sha1.h sha512.c sha512.h fixedint.h
endif
idevicerestore_CFLAGS = $(AM_CFLAGS)
idevicerestore_LDFLAGS = $(AM_LDFLAGS)
idevicerestore_LDADD = $(AM_LDADD)
