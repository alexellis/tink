FROM registry:2.6.2
RUN apk add --no-cache --update curl
ARG REGISTRY_USERNAME
ARG REGISTRY_PASSWORD
RUN mkdir -p /certs /auth
RUN htpasswd -Bbn ${REGISTRY_USERNAME} ${REGISTRY_PASSWORD} > /auth/htpasswd
EXPOSE 443
