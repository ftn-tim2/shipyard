FROM alpine:latest
RUN apk add --update git ca-certificates && \
    rm -rf /var/cache/apk/*
ADD static /static
ADD . /bin/controller
RUN chmod +x /bin/controller
EXPOSE 8080
ENTRYPOINT ["/bin/controller"]
