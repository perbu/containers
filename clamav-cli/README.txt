
# To build
docker build --tag=clamav .


# Invocation, might need a wrapper.
docker run --mount type=bind,source=/tmp/data,target=/data clamav /data/random
