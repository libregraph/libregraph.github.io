# Components of LibreGraph

## Identity & Authorization

LibreGraph is designed for environments where users are managed in an LDAP tree. If the current environment does not provide an LDAP [LibreGraph IDM](https://github.com/libregraph/idm) can be used as a drop in replacement for OpenLDAP.

Check the [Kopano Identity Management Daemon](https://github.com/Kopano-dev/kidm) for a practical implementation of LibreGraph IDM.

Authorization of users is handled through OpenID Connect, which is provided by [LibreGraph Connect (LICO)](https://github.com/libregraph/lico).

## API Gateway

[The LibreGraph API Gateway (LIGA)](https://github.com/libregraph/liga) provides a common endpoint to interface with various HTTP based backend APIs. The availability of APIS is controlled by plugins. See the [plugin section in the Liga readme for more details](https://github.com/libregraph/liga#plugins).

## Groupware RestAPI

[The LibreGraph Groupware RestAPI (GRAPI)](https://github.com/libregraph/grapi) provides a general REST web service for multiple groupware applications/standards. It aims to be largely compatible with Microsoft Graph. See [COMPAT](https://github.com/libregraph/grapi/blob/master/COMPAT.md) for compatibility details.

GRAPI is meant to be used directly by LIGA and requires Python 3. The endpoints exposed by GRAPI can map multiple data provider backends into the same API using backend implementations. See the [Backends](https://github.com/libregraph/grapi#backends) section below for details.
