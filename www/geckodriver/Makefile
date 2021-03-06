# $OpenBSD: Makefile,v 1.6 2020/03/12 10:30:05 semarie Exp $

COMMENT =	W3C webdriver for Gecko-based browsers

GH_ACCOUNT =	mozilla
GH_PROJECT =	geckodriver
GH_TAGNAME =	v0.22.0
REVISION =	0

CATEGORIES =	www

MAINTAINER =	Aaron Bieber <abieber@openbsd.org>

# mozilla public license
PERMIT_PACKAGE =	Yes

DISTFILES +=		${DISTNAME}${EXTRACT_SUFX}

MODULES =		devel/cargo

CONFIGURE_STYLE =	cargo
SEPARATE_BUILD =	Yes

# keep libc >=0.2.63 for sparc64 support
MODCARGO_CRATES_UPDATE +=	libc
MODCARGO_CRATES +=	libc	0.2.63	# MIT/Apache-2.0

MODCARGO_CRATES +=	adler32	1.0.3		# BSD-3-Clause AND Zlib
MODCARGO_CRATES +=	aho-corasick	0.6.8		# Unlicense/MIT
MODCARGO_CRATES +=	arrayvec	0.4.7		# MIT/Apache-2.0
MODCARGO_CRATES +=	base64	0.9.3		# MIT/Apache-2.0
MODCARGO_CRATES +=	bitflags	1.0.4		# MIT/Apache-2.0
MODCARGO_CRATES +=	build_const	0.2.1		# MIT
MODCARGO_CRATES +=	byteorder	1.2.6		# Unlicense/MIT
MODCARGO_CRATES +=	bytes	0.4.10		# MIT
MODCARGO_CRATES +=	bzip2	0.3.3		# MIT/Apache-2.0
MODCARGO_CRATES +=	bzip2-sys	0.1.6		# MIT/Apache-2.0
MODCARGO_CRATES +=	cc	1.0.25		# MIT/Apache-2.0
MODCARGO_CRATES +=	cfg-if	0.1.5		# MIT/Apache-2.0
MODCARGO_CRATES +=	chrono	0.2.25		# MIT/Apache-2.0
MODCARGO_CRATES +=	clap	2.32.0		# MIT
MODCARGO_CRATES +=	cloudabi	0.0.3		# BSD-2-Clause
MODCARGO_CRATES +=	cookie	0.11.0		# MIT/Apache-2.0
MODCARGO_CRATES +=	crc	1.8.1		# MIT OR Apache-2.0
MODCARGO_CRATES +=	crossbeam-deque	0.6.1		# MIT/Apache-2.0
MODCARGO_CRATES +=	crossbeam-epoch	0.5.2		# MIT/Apache-2.0
MODCARGO_CRATES +=	flate2	1.0.2		# MIT/Apache-2.0
MODCARGO_CRATES +=	crossbeam-utils	0.5.0		# MIT/Apache-2.0
MODCARGO_CRATES +=	fnv	1.0.6		# Apache-2.0 / MIT
MODCARGO_CRATES +=	fuchsia-zircon	0.3.3		# BSD-3-Clause
MODCARGO_CRATES +=	fuchsia-zircon-sys	0.3.3		# BSD-3-Clause
MODCARGO_CRATES +=	futures	0.1.24		# MIT/Apache-2.0
MODCARGO_CRATES +=	futures-cpupool	0.1.8		# MIT/Apache-2.0
MODCARGO_CRATES +=	h2	0.1.12		# MIT
MODCARGO_CRATES +=	http	0.1.13		# MIT/Apache-2.0
MODCARGO_CRATES +=	httparse	1.3.2		# MIT/Apache-2.0
MODCARGO_CRATES +=	hyper	0.12.10		# MIT
MODCARGO_CRATES +=	idna	0.1.5		# MIT/Apache-2.0
MODCARGO_CRATES +=	indexmap	1.0.1		# Apache-2.0/MIT
MODCARGO_CRATES +=	iovec	0.1.2		# MIT/Apache-2.0
MODCARGO_CRATES +=	itoa	0.4.3		# MIT/Apache-2.0
MODCARGO_CRATES +=	kernel32-sys	0.2.2		# MIT
MODCARGO_CRATES +=	lazy_static	1.1.0		# MIT/Apache-2.0
MODCARGO_CRATES +=	lazycell	1.1.0		# MIT/Apache-2.0
#MODCARGO_CRATES +=	libc	0.2.43		# MIT/Apache-2.0
MODCARGO_CRATES +=	lock_api	0.1.3		# Apache-2.0/MIT
MODCARGO_CRATES +=	log	0.4.5		# MIT/Apache-2.0
MODCARGO_CRATES +=	mio	0.6.16		# MIT
MODCARGO_CRATES +=	matches	0.1.8		# MIT
MODCARGO_CRATES +=	memchr	2.0.2		# Unlicense/MIT
MODCARGO_CRATES +=	memoffset	0.2.1		# MIT
MODCARGO_CRATES +=	miniz_oxide	0.1.3		# MIT
MODCARGO_CRATES +=	miniz_oxide_c_api	0.1.3		# MIT
MODCARGO_CRATES +=	mio-uds	0.6.7		# MIT/Apache-2.0
MODCARGO_CRATES +=	miow	0.2.1		# MIT/Apache-2.0
MODCARGO_CRATES +=	mozprofile	0.4.0		# MPL-2.0
MODCARGO_CRATES +=	mozrunner	0.8.0		# MPL-2.0
MODCARGO_CRATES +=	mozversion	0.1.3		# MPL-2.0
MODCARGO_CRATES +=	msdos_time	0.1.6		# MIT OR Apache-2.0
MODCARGO_CRATES +=	net2	0.2.33		# MIT/Apache-2.0
MODCARGO_CRATES +=	nodrop	0.1.12		# MIT/Apache-2.0
MODCARGO_CRATES +=	num	0.1.42		# MIT/Apache-2.0
MODCARGO_CRATES +=	num-integer	0.1.39		# MIT/Apache-2.0
MODCARGO_CRATES +=	num-iter	0.1.37		# MIT/Apache-2.0
MODCARGO_CRATES +=	num-traits	0.2.6		# MIT/Apache-2.0
MODCARGO_CRATES +=	num_cpus	1.8.0		# MIT/Apache-2.0
MODCARGO_CRATES +=	owning_ref	0.3.3		# MIT
MODCARGO_CRATES +=	parking_lot	0.6.4		# Apache-2.0/MIT
MODCARGO_CRATES +=	parking_lot_core	0.3.1		# Apache-2.0/MIT
MODCARGO_CRATES +=	percent-encoding	1.0.1		# MIT/Apache-2.0
MODCARGO_CRATES +=	podio	0.1.6		# MIT OR Apache-2.0
MODCARGO_CRATES +=	proc-macro2	0.4.19		# MIT/Apache-2.0
MODCARGO_CRATES +=	quote	0.6.8		# MIT/Apache-2.0
MODCARGO_CRATES +=	rand	0.3.22		# MIT/Apache-2.0
MODCARGO_CRATES +=	rand	0.4.3		# MIT/Apache-2.0
MODCARGO_CRATES +=	rand	0.5.5		# MIT/Apache-2.0
MODCARGO_CRATES +=	rand_core	0.2.1		# MIT/Apache-2.0
MODCARGO_CRATES +=	redox_syscall	0.1.40		# MIT
MODCARGO_CRATES +=	regex	0.2.11		# MIT/Apache-2.0
MODCARGO_CRATES +=	regex	1.0.5		# MIT/Apache-2.0
MODCARGO_CRATES +=	regex-syntax	0.5.6		# MIT/Apache-2.0
MODCARGO_CRATES +=	regex-syntax	0.6.2		# MIT/Apache-2.0
MODCARGO_CRATES +=	remove_dir_all	0.5.1		# MIT/Apache-2.0
MODCARGO_CRATES +=	rust-ini	0.10.3		# MIT
MODCARGO_CRATES +=	rustc_version	0.2.3		# MIT/Apache-2.0
MODCARGO_CRATES +=	ryu	0.2.6		# Apache-2.0 OR BSL-1.0
MODCARGO_CRATES +=	safemem	0.3.0		# MIT/Apache-2.0
MODCARGO_CRATES +=	scopeguard	0.3.3		# MIT/Apache-2.0
MODCARGO_CRATES +=	semver	0.6.0		# MIT/Apache-2.0
MODCARGO_CRATES +=	semver	0.9.0		# MIT/Apache-2.0
MODCARGO_CRATES +=	semver-parser	0.7.0		# MIT/Apache-2.0
MODCARGO_CRATES +=	serde	1.0.79		# MIT/Apache-2.0
MODCARGO_CRATES +=	serde_derive	1.0.79		# MIT/Apache-2.0
MODCARGO_CRATES +=	serde_json	1.0.27		# MIT/Apache-2.0
MODCARGO_CRATES +=	slab	0.4.1		# MIT
MODCARGO_CRATES +=	smallvec	0.6.5		# MIT/Apache-2.0
MODCARGO_CRATES +=	stable_deref_trait	1.1.1		# MIT/Apache-2.0
MODCARGO_CRATES +=	string	0.1.1		# MIT
MODCARGO_CRATES +=	strsim	0.7.0		# MIT
MODCARGO_CRATES +=	syn	0.15.4		# MIT/Apache-2.0
MODCARGO_CRATES +=	tempdir	0.3.7		# MIT/Apache-2.0
MODCARGO_CRATES +=	term_size	0.3.1		# MIT/Apache-2.0
MODCARGO_CRATES +=	textwrap	0.10.0		# MIT
MODCARGO_CRATES +=	thread_local	0.3.6		# Apache-2.0/MIT
MODCARGO_CRATES +=	time	0.1.40		# MIT/Apache-2.0
MODCARGO_CRATES +=	tokio	0.1.8		# MIT
MODCARGO_CRATES +=	tokio-codec	0.1.0		# MIT
MODCARGO_CRATES +=	tokio-current-thread	0.1.1		# MIT
MODCARGO_CRATES +=	tokio-executor	0.1.4		# MIT
MODCARGO_CRATES +=	tokio-fs	0.1.3		# MIT
MODCARGO_CRATES +=	tokio-io	0.1.8		# MIT
MODCARGO_CRATES +=	tokio-reactor	0.1.5		# MIT
MODCARGO_CRATES +=	tokio-tcp	0.1.1		# MIT
MODCARGO_CRATES +=	tokio-threadpool	0.1.6		# MIT
MODCARGO_CRATES +=	tokio-timer	0.2.6		# MIT
MODCARGO_CRATES +=	tokio-udp	0.1.2		# MIT
MODCARGO_CRATES +=	tokio-uds	0.2.1		# MIT
MODCARGO_CRATES +=	try-lock	0.2.2		# MIT
MODCARGO_CRATES +=	ucd-util	0.1.1		# MIT/Apache-2.0
MODCARGO_CRATES +=	unicode-bidi	0.3.4		# MIT / Apache-2.0
MODCARGO_CRATES +=	unicode-normalization	0.1.7		# MIT/Apache-2.0
MODCARGO_CRATES +=	unicode-segmentation	1.2.1		# MIT/Apache-2.0
MODCARGO_CRATES +=	unicode-width	0.1.5		# MIT/Apache-2.0
MODCARGO_CRATES +=	unicode-xid	0.1.0		# MIT/Apache-2.0
MODCARGO_CRATES +=	unreachable	1.0.0		# MIT / Apache-2.0
MODCARGO_CRATES +=	url	1.7.1		# MIT/Apache-2.0
MODCARGO_CRATES +=	uuid	0.5.1		# MIT/Apache-2.0
MODCARGO_CRATES +=	utf8-ranges	1.0.1		# Unlicense/MIT
MODCARGO_CRATES +=	version_check	0.1.4		# MIT/Apache-2.0
MODCARGO_CRATES +=	void	1.0.2		# MIT
MODCARGO_CRATES +=	want	0.0.6		# MIT
MODCARGO_CRATES +=	webdriver	0.37.0		# MPL-2.0
MODCARGO_CRATES +=	winapi	0.2.8		# MIT
MODCARGO_CRATES +=	winapi	0.3.5		# MIT/Apache-2.0
MODCARGO_CRATES +=	winapi-build	0.1.1		# MIT
MODCARGO_CRATES +=	winapi-i686-pc-windows-gnu	0.4.0		# MIT/Apache-2.0
MODCARGO_CRATES +=	winapi-x86_64-pc-windows-gnu	0.4.0		# MIT/Apache-2.0
MODCARGO_CRATES +=	winreg	0.5.1		# MIT
MODCARGO_CRATES +=	ws2_32-sys	0.2.1		# MIT
MODCARGO_CRATES +=	zip	0.3.3		# MIT

LIB_DEPENDS +=	archivers/bzip2
WANTLIB += c c++abi m pthread bz2

.include <bsd.port.mk>
