FROM alpine:3.7
RUN apk add --no-cache outils-sha256
ENTRYPOINT ["/usr/bin/sha256"]
# The default is to checksum this thing
CMD ["/data/random"]
