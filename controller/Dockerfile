FROM alpine:latest
RUN apk add --update git ca-certificates && \
    rm -rf /var/cache/apk/*
ADD static /static
RUN mkdir /bin/controller
ADD controller /bin/controller
EXPOSE 8080
ENTRYPOINT ["/bin/controller"]
