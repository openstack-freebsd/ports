# Created by: Alexander Nusov <alexander.nusov@nfvexpress.com>
# $FreeBSD: head/devel/py-os-client-config/Makefile 432753 2017-01-29 14:48:53Z novel $

PORTNAME=	os-client-config
PORTVERSION=	1.28.0
CATEGORIES=	devel python
MASTER_SITES=	CHEESESHOP
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	skonmeme@gmail.com
COMMENT=	OpenStack Client Configuation Library

LICENSE=	APACHE20

BUILD_DEPENDS=	${PYTHON_PKGNAMEPREFIX}pbr>=2.0.0:devel/py-pbr
RUN_DEPENDS=	${PYTHON_PKGNAMEPREFIX}yaml>=3.1.0:devel/py-yaml \
		${PYTHON_PKGNAMEPREFIX}appdirs>=1.3.0:devel/py-appdirs \
		${PYTHON_PKGNAMEPREFIX}keystoneauth1>=2.1.0:devel/py-keystoneauth1 \
		${PYTHON_PKGNAMEPREFIX}requestsexceptions>=1.1.1:devel/py-requestsexceptions

USES=		python
USE_PYTHON=	distutils autoplist noegginfo
NO_ARCH=	yes

.include <bsd.port.mk>
