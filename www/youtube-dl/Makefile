# $OpenBSD: Makefile,v 1.211 2020/07/28 15:14:33 kn Exp $

COMMENT =	CLI program to download videos from YouTube and other sites

VERSION =	2020.07.28
MODPY_EGG_VERSION =	${VERSION:S/.0/./g}

DISTNAME =	youtube-dl-${VERSION}
CATEGORIES =	www

HOMEPAGE =	https://ytdl-org.github.io/youtube-dl/

MAINTAINER =	Paul Irofti <paul@irofti.net>

# Public Domain
PERMIT_PACKAGE =	Yes

MASTER_SITES =	https://youtube-dl.org/downloads/${VERSION}/

MODULES =	lang/python

MODPY_SETUPTOOLS =	Yes
MODPY_VERSION =	${MODPY_DEFAULT_VERSION_3}

TEST_DEPENDS +=	devel/flake8 \
		devel/py-nose${MODPY_FLAVOR}

TEST_ENV =	PATH=${PORTPATH}

pre-test:
	ln -sf ${LOCALBASE}/bin/nosetests${MODPY_BIN_SUFFIX} \
	    ${WRKDIR}/bin/nosetests

do-test:
	${TEST_ENV} ${MAKE_PROGRAM} -C ${WRKSRC} ${TEST_TARGET}

WRKDIST =	${WRKDIR}/youtube-dl

.include <bsd.port.mk>
