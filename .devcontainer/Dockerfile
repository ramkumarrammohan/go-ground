FROM golang:1.15-alpine3.12

# Configure to reduce warnings and limitations as instruction from official VSCode Remote-Containers.
# See https://code.visualstudio.com/docs/remote/containers-advanced#_reducing-dockerfile-build-warnings.
ENV DEBIAN_FRONTEND=noninteractive
RUN apk update 

# Dev tools installation
RUN apk add git

# Revert workaround at top layer.
ENV DEBIAN_FRONTEND=dialog

# Expose service ports.
# EXPOSE 9999