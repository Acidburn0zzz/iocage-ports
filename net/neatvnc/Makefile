# $FreeBSD$

PORTNAME=	neatvnc
PORTVERSION=	s20200113
CATEGORIES=	net

MAINTAINER=	jbeich@FreeBSD.org
COMMENT=	Liberally licensed VNC server library

LICENSE=	ISCL
LICENSE_FILE=	${WRKSRC}/COPYING

BUILD_DEPENDS=	${LOCALBASE}/include/libdrm/drm_fourcc.h:graphics/libdrm
LIB_DEPENDS=	libuv.so:devel/libuv

USES=		compiler:c11 meson pkgconfig xorg
USE_GITHUB=	yes
USE_XORG=	pixman
USE_LDCONFIG=	yes
GH_ACCOUNT=	any1
GH_TAGNAME=	6bb3362

OPTIONS_DEFINE=	JPEG
OPTIONS_DEFAULT=JPEG

JPEG_LIB_DEPENDS=	libturbojpeg.so:graphics/libjpeg-turbo
JPEG_MESON_ENABLED=	tight-encoding

.include <bsd.port.mk>
