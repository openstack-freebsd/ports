# Created by: Alexander Nusov <alexander.nusov@nfvexpress.com>
# $FreeBSD: head/devel/py-wsme/Makefile 432702 2017-01-29 08:59:19Z novel $

PORTNAME=	wsme
PORTVERSION=	0.9.2
CATEGORIES=	devel python
MASTER_SITES=	CHEESESHOP
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}
DISTNAME=	WSME-${PORTVERSION}

MAINTAINER=	skonmeme@gmail.com
COMMENT=	Simplify the writing of REST APIs

BUILD_DEPENDS=	${PYTHON_PKGNAMEPREFIX}pbr>=2.0.0:devel/py-pbr
RUN_DEPENDS=	${PYTHON_PKGNAMEPREFIX}six>=1.9.0:devel/py-six \
		${PYTHON_PKGNAMEPREFIX}webob>=1.2.3:www/py-webob \
		${PYTHON_PKGNAMEPREFIX}simplegeneric>=0:devel/py-simplegeneric \
		${PYTHON_PKGNAMEPREFIX}pytz>=0:devel/py-pytz \
		${PYTHON_PKGNAMEPREFIX}netaddr>=0.7.12:net/py-netaddr

NO_ARCH=	yes

USES=		python
USE_PYTHON=	autoplist distutils

.include <bsd.port.mk>
