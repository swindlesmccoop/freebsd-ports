PORTNAME =			cmixer
DISTVERSION =		0.3
CATEGORIES =		audio
MAINTAINER =		swindlesmccoop@waifu.club
COMMENT =			simple curses mixer
WWW = 				https://rhaalovely.net/stuff/
MASTER_SITES =		${WWW}

NO_BUILD =			yes
NO_TEST = 			yes

#RUN_DEPENDS =		devel/p5-Curses-UI

INTERPRETER_PATCH =	${PATCHDIR}/interpreter.patch
PLIST_FILES =		bin/cmixer

do-install:
	cp ${WRKSRC}/cmixer.pl ${WRKSRC}/cmixer.pl.new
	patch ${WRKSRC}/cmixer.pl.new < ${INTERPRETER_PATCH}
	install ${WRKSRC}/cmixer.pl.new ${WRKSRC}/../stage/usr/local/bin/cmixer

.include <bsd.port.mk>