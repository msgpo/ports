# $OpenBSD: Makefile,v 1.8 2020/01/16 20:21:15 jasper Exp $

COMMENT=		C++ wrapper for the libxml XML parser library

GNOME_VERSION=		3.2.0
GNOME_PROJECT=		libxml++
PKGNAME=		${GNOME_PROJECT}3-${GNOME_VERSION}

SHARED_LIBS +=  xml++-3.0            0.1      # 1.0

CATEGORIES=		textproc

HOMEPAGE=		http://libxmlplusplus.sourceforge.net/

MAINTAINER=		Jasper Lievisse Adriaanse <jasper@openbsd.org>, \
			Antoine Jacoutot <ajacoutot@openbsd.org>

# LGPLv2.1+
PERMIT_PACKAGE=	Yes

WANTLIB += ffi glib-2.0 glibmm-2.4 gmodule-2.0 gobject-2.0 iconv
WANTLIB += intl lzma m pcre pthread sigc-2.0 xml2 z
WANTLIB += ${COMPILER_LIBCXX}

MODULES=		x11/gnome

DEBUG_PACKAGES =	${BUILD_PACKAGES}

# c++11
COMPILER =		base-clang ports-gcc

LIB_DEPENDS=		devel/glib2mm \
			textproc/libxml

CONFIGURE_STYLE=	gnu

.include <bsd.port.mk>
