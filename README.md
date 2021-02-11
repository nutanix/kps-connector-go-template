# Karbon Platform Services (KPS) Connector Go Template
Welcome to the Golang template for building KPS Connectors. This template is an opinionated implementation of the
gRPC service contract defined in [KPS Connector IDL](https://github.com/nutanix/kps-connector-idl) built using the
[KPS Connector Go SDK](https://github.com/nutanix/kps-connector-idl).

## Usage
- Start by cloning this repo
- Copy all the contents into another repo in which you intend to build the connector
- Fill in the `TODO` blocks in `connector/template.go` and the connector name in `connector/config.go`
- Replace the default values marked with `TODO` comments for connector name, docker repository uri, and docker image tag in `Makefile`
- Change the module name in `go.mod` file

## Building
- Run `make build`

## Publishing
- Ensure you have `docker push` access to your docker registry
- Run `make publish`
