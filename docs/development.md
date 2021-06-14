# Development

## Architecture

![Architecture overview](img/architecture.drawio.svg "Architecture overview of LibreGraph")

## Backends

LibreGraph was designed with a plug-able backend system in mind. Backends can be mixed (e.g. one backend for calendar data and one for file data) and backends providing the same kind of data (e.g. Kopano and IMAP for mail access) can even be used at the same time.

### Kopano

State: In active development

Full groupware backend using the Kopano Groupware as storage.

### CalDAV

State: proof of concept

### IMAP

State: proof of concept

### LDAP

State: proof of concept

Capable of a read-only presentation of shared contacts.

### Mock

Empty backend for testing

### Write your own

TODO

## Contribute

Join the [discussion](https://github.com/LibreGraph/libregraph.github.io/discussions)!
