FROM alpine:3.15

RUN apk update && apk add bash openssl && wget -qO /peer-finder http://storage.googleapis.com/kubernetes-release/pets/peer-finder

ENTRYPOINT ["/install.sh"]

COPY install.sh /

RUN chmod -c 755 /install.sh /peer-finder
