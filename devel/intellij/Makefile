# $OpenBSD: Makefile,v 1.69 2020/07/12 07:29:18 rsadowski Exp $

COMMENT=		IntelliJ IDEA Java IDE

V=			2020.1.3
DISTNAME=		ideaIC-${V}
PKGNAME=		intellij-${V}
CATEGORIES=		devel

HOMEPAGE=		https://www.jetbrains.com/idea/
MAINTAINER=		Lucas Raab <tuftedocelot@fastmail.fm>

# Apache v2.0
PERMIT_PACKAGE=	Yes

MASTER_SITES=		https://download.jetbrains.com/idea/

MODULES=		java
MODJAVA_VER=		11

BUILD_DEPENDS=		${MODJAVA_RUN_DEPENDS}

RUN_DEPENDS=		devel/desktop-file-utils \
			java/javaPathHelper

NO_TEST=		Yes

WRKDIST=		${WRKDIR}/idea-IC-201.8538.31
IJ=			${PREFIX}/intellij

# If NO_BUILD is set, JAVA_HOME doesn't get defined. So do
# a no-op for do-build.
do-build:
	@true

do-install:
	${INSTALL_DATA_DIR} ${IJ}
	cd ${WRKDIST} && pax -rw . ${IJ}
	@rm -rf ${IJ}/bin/libdbm64.so
	@rm -rf ${IJ}/jbr
	@rm -rf ${IJ}/plugins/android
	@${SUBST_PROGRAM} ${FILESDIR}/idea ${PREFIX}/bin/idea
	@ln -s ${TRUEPREFIX}/bin/idea ${PREFIX}/bin/intellij
	${INSTALL_MAN} ${FILESDIR}/idea.1 ${PREFIX}/man/man1
	${INSTALL_DATA_DIR} ${PREFIX}/share/applications
	cd ${WRKDIST}/lib && ${JAVA_HOME}/bin/jar xf icons.jar
	${INSTALL_DATA} ${WRKDIST}/lib/icon.png ${IJ}/idea.png
	@${SUBST_DATA} ${FILESDIR}/intellij.desktop \
		${PREFIX}/share/applications/intellij.desktop

.include <bsd.port.mk>
