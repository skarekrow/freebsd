# $FreeBSD$

PACKAGE=runtime
PROG=	rc-update
SRCS=	rc-update.c \
       	${.CURDIR}/../../contrib/openrc/rc-misc.c \
       	${.CURDIR}/../../contrib/openrc/_usage.c
CFLAGS+=	-I${.CURDIR}/../../contrib/openrc \
	       	-I${.CURDIR}/../../lib/libeinfo \
	       	-I${.CURDIR}/../../lib/librc \
	       	-I${.CURDIR}/../../include

WARNS?=	3
MAN=	rc-update.8

LIBADD=	einfo rc util

.include <bsd.prog.mk>
