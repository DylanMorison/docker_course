# Specify a base image
FROM node:alpine

# Specify the working directory of the container
# all files will be copied here instead of root dir
WORKDIR /usr/app

# Copy package.json to /user/app
COPY ./package.json ./
# Install all deps
RUN npm install
# Copy everything else to avoid running npm install when it is 
# not necesary. The only siutation in which npm install would be run is 
# if something in package.json has changed.
COPY ./ ./ 

# Default command
CMD ["npm", "start"]