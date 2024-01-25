# NEAR Dev Containers

A collection of dev containers and features designed for working with NEAR in various contexts.

## Usage

To use a feature from this repository, add it to a devcontainer.json. You can read more about devcontainer features here: https://containers.dev/features

## Compatibility

Note that all these images depend on having the rust feature set up (`ghcr.io/devcontainers/features/rust:1`), as well as using either `debian:latest` or `ubuntu:latest` as the base image since the default devcontainer image causes issues with permissions.

## Features

| Feature | OCI Image | Description |
| Cargo Near | TODO | Installs [Cargo Near](https://github.com/near/cargo-near) - Cargo extension for building near-sdk-rs smart contracts and ABI schemas on NEAR |
