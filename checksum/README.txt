
# To build
docker build --tag=lol .


# Invocation, might need a wrapper.
docker run --mount type=bind,source=/tmp/data,target=/data lol /data/random
