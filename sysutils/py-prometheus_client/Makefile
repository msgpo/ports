# $OpenBSD: Makefile,v 1.6 2020/07/03 21:13:11 sthen Exp $

COMMENT =		python client for the prometheus monitoring system

MODPY_EGG_VERSION =	0.7.1
DISTNAME =		prometheus_client-${MODPY_EGG_VERSION}
PKGNAME =		py-${DISTNAME}
REVISION =		2

CATEGORIES =		sysutils

HOMEPAGE =		https://github.com/prometheus/client_python

# Apache License v2
PERMIT_PACKAGE =	Yes

MODULES =		lang/python
MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes

FLAVORS =		python3
FLAVOR =		python3

NO_TEST =		Yes

.include <bsd.port.mk>
