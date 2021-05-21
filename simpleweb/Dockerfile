# Specify a base image
FROM node:alpine

# Specify the working directory of the container
WORKDIR /usr/app

# Install some dependencies
COPY ./ ./
RUN npm install

# Default command
CMD ["npm", "start"]