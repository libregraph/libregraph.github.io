# Components of LibreGraph

## Identity & Authorization

LibreGraph is designed for environments where users are managed in an LDAP tree. If the current environment does not provide an LDAP [LibreGraph IDM](https://github.com/libregraph/idm) can be used as a drop in replacement for OpenLDAP.

Check the [Kopano Identity Management Daemon](https://github.com/Kopano-dev/kidm) for a practical implementation of LibreGraph IDM.

Authorization of users is handled through OpenID Connect, which is provided by [LibreGraph Connect (lico)](https://github.com/libregraph/lico).

## API Gateway

