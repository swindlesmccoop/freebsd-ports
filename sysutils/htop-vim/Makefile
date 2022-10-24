PORTNAME =			htop-vim
DISTVERSION =		3.2.1
CATEGORIES =		sysutils
REVISION = 			2
MAINTAINER =		swindlesmccoop@waifu.club
COMMENT =			Interactive process viewer with vim-like keybindings

LICENSE=	GPLv2
LICENSE_FILE=	${WRKSRC}/COPYING

USES=		autoreconf compiler:c11 cpe libtool localbase ncurses pkgconfig \
		python:build shebangfix

MASTER_SITES = https://swindlesmccoop.xyz/misc/

GNU_CONFIGURE=	yes
#CONFIGURE_ARGS=	--enable-unicode
CONFIGURE_ARGS +=	--disable-unicode --disable-taskstats

PLIST_FILES=	bin/htop \
		man/man1/htop.1 \
		share/applications/htop.desktop \
		share/icons/hicolor/scalable/apps/htop.svg \
		share/pixmaps/htop.png

.include <bsd.port.mk>
