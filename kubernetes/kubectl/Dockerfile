FROM alpine:3.11

WORKDIR /work

ARG KUBE_VERSION=1.16.1

ENV KUBE_VERSION $KUBE_VERSION

ADD https://storage.googleapis.com/kubernetes-release/release/v${KUBE_VERSION}/bin/linux/amd64/kubectl /usr/local/bin/kubectl

RUN chmod +x /usr/local/bin/kubectl \
    && apk add --no-cache gettext curl jq
