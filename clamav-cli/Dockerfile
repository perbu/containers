FROM alpine:3.7
RUN apk add --no-cache clamav wget
RUN wget -O /var/lib/clamav/main.cvd http://database.clamav.net/main.cvd && \
    wget -O /var/lib/clamav/daily.cvd http://database.clamav.net/daily.cvd && \
    wget -O /var/lib/clamav/bytecode.cvd http://database.clamav.net/bytecode.cvd && \
    chown clamav:clamav /var/lib/clamav/*.cvd
COPY freshscan /usr/local/bin/freshscan
ENTRYPOINT ["/usr/local/bin/freshscan"]
# The default is to scan this thing
CMD ["/data/random"]
