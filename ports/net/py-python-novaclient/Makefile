# Created by: Roman Bogorodskiy <novel@FreeBSD.org>
# $FreeBSD: head/net/py-python-novaclient/Makefile 428767 2016-12-17 15:31:09Z novel $

PORTNAME=	python-novaclient
PORTVERSION=	9.1.1
CATEGORIES=	net python
MASTER_SITES=	CHEESESHOP
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	skonmeme@gmail.com
COMMENT=	Client for the OpenStack Nova API

BUILD_DEPENDS=	${PYTHON_PKGNAMEPREFIX}pbr>=2.0.0:devel/py-pbr
RUN_DEPENDS=	${PYTHON_PKGNAMEPREFIX}keystoneauth1>=3.0.1:devel/py-keystoneauth1 \
		${PYTHON_PKGNAMEPREFIX}iso8601>=0.1.11:devel/py-iso8601 \
		${PYTHON_PKGNAMEPREFIX}oslo.i18n>=2.1.0:devel/py-oslo.i18n \
		${PYTHON_PKGNAMEPREFIX}oslo.serialization>=1.10.0:devel/py-oslo.serialization \
		${PYTHON_PKGNAMEPREFIX}oslo.utils>=3.20.0:devel/py-oslo.utils \
		${PYTHON_PKGNAMEPREFIX}prettytable>=0.7.1:devel/py-prettytable \
		${PYTHON_PKGNAMEPREFIX}simplejson>=2.2.0:devel/py-simplejson \
		${PYTHON_PKGNAMEPREFIX}six>=1.9.0:devel/py-six \
		${PYTHON_PKGNAMEPREFIX}Babel>=2.3.4:devel/py-babel

USES=		python shebangfix
SHEBANG_FILES=	novaclient/tests/functional/hooks/post_test_hook.sh
USE_PYTHON=	distutils autoplist noegginfo
NO_ARCH=	yes

post-patch:
	@${REINPLACE_CMD} -e 's,install_requires.*,,' ${WRKSRC}/setup.py

.include <bsd.port.mk>
