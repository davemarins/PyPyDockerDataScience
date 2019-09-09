FROM alpine:latest

# Updates
RUN apk update
RUN apk add --no-cache \
        perl \
        wget \
        openssl \
        ca-certificates \
        libc6-compat \
        libstdc++
RUN mkdir Hello
COPY cmake-build-debug/Cpp /Hello
WORKDIR Hello
RUN chmod 755 Cpp

CMD ["./Cpp"]
