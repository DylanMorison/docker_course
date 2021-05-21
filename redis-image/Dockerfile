# Use an existing docker image as a base
FROM alpine

# Download and install a dep
RUN apk add --update redis
RUN apk add --update gcc

# Tell the image what todo when it starts
# as a container
CMD ["redis-server"]