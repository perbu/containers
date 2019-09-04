
# To build
docker build --tag=lol .


# Invocation, might need a wrapper.
docker run --mount type=bind,source=/Users/perbu/Docker/checksum/files,target=/data lol /data/random
