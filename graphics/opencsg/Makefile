# $OpenBSD: Makefile,v 1.14 2020/02/05 19:22:26 rsadowski Exp $

COMMENT =		constructive solid geometry rendering library

V =			1.4.2
DISTNAME =		OpenCSG-${V}
PKGNAME =		opencsg-${V}
REVISION =		0

SHARED_LIBS =		opencsg		1.0

CATEGORIES =		graphics

HOMEPAGE =		http://www.opencsg.org/

# GPLv2 with CGAL exception
PERMIT_PACKAGE =	Yes

WANTLIB += ${COMPILER_LIBCXX} GL GLEW m

MASTER_SITES =		http://www.opencsg.org/

MODULES =		devel/qmake \
			x11/qt5

SEPARATE_BUILD =	No

LIB_DEPENDS =		graphics/glew

WRKSRC =		${WRKDIST}/src

pre-configure:
	${SUBST_CMD} ${WRKSRC}/src.pro

do-install:
	${INSTALL_DATA} ${WRKDIST}/lib/libopencsg.so.${LIBopencsg_VERSION} \
		${PREFIX}/lib
	${INSTALL_DATA} ${WRKDIST}/include/opencsg.h ${PREFIX}/include

.include <bsd.port.mk>
