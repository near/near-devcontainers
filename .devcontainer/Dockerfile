ARG VARIANT="3.12"
FROM mcr.microsoft.com/vscode/devcontainers/base:0-alpine-${VARIANT}

# Additional packages:
# - libudev-dev: required for the hidapi crate (cargo-near dependency)
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends libudev-dev