# Created by: Alexander Nusov <alexander.nusov@nfvexpress.com>
# $FreeBSD: head/net/py-python-keystoneclient/Makefile 432756 2017-01-29 15:15:45Z novel $

PORTNAME=	python-keystoneclient
PORTVERSION=	3.13.0
CATEGORIES=	net python
MASTER_SITES=	CHEESESHOP
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	skonmeme@gmail.com
COMMENT=	Client for the OpenStack Keystone API

LICENSE=	APACHE20

BUILD_DEPENDS=	${PYTHON_PKGNAMEPREFIX}pbr>=2.0.0:devel/py-pbr
RUN_DEPENDS=	${PYTHON_PKGNAMEPREFIX}debtcollector>=1.2.0:devel/py-debtcollector \
		${PYTHON_PKGNAMEPREFIX}keystoneauth1>=3.0.1:devel/py-keystoneauth1 \
		${PYTHON_PKGNAMEPREFIX}oslo.config>=4.0.0:devel/py-oslo.config \
		${PYTHON_PKGNAMEPREFIX}oslo.i18n>=2.1.0:devel/py-oslo.i18n \
		${PYTHON_PKGNAMEPREFIX}oslo.serialization>=1.10.0:devel/py-oslo.serialization \
		${PYTHON_PKGNAMEPREFIX}oslo.utils>=3.20.0:devel/py-oslo.utils \
		${PYTHON_PKGNAMEPREFIX}positional>=1.1.1:devel/py-positional \
		${PYTHON_PKGNAMEPREFIX}requests>=2.14.2:www/py-requests \
		${PYTHON_PKGNAMEPREFIX}six>=1.9.0:devel/py-six \
		${PYTHON_PKGNAMEPREFIX}stevedore>=1.20.0:devel/py-stevedore

USES=		python shebangfix
SHEBANG_FILES=	keystoneclient/tests/functional/hooks/post_test_hook.sh
USE_PYTHON=	distutils autoplist noegginfo
NO_ARCH=	yes

post-patch:
	@${REINPLACE_CMD} -e 's,install_requires.*,,' ${WRKSRC}/setup.py

.include <bsd.port.mk>
