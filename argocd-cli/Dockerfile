FROM alpine:latest

ARG ARGOCD_VERSION=v1.0.0
ENV USER=root

RUN apk add --no-cache wget ca-certificates && \
    wget https://github.com/argoproj/argo-cd/releases/download/$ARGOCD_VERSION/argocd-linux-amd64 && \
    mv ./argocd-linux-amd64 /usr/bin/argocd && \
    chmod 755 /usr/bin/argocd && \
    apk del wget
