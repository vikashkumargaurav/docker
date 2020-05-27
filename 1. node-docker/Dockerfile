# Specify a base image
FROM node:12.16.3-alpine3.11

# By specifying the dir path we are specifing that any further command will be  executed relative to  this path inside container
WORKDIR /app

# copy package.json
COPY package.json ./

# Install some dependencies
RUN npm install

# Copy curr folder to the container
COPY ./ ./

# Default command after start
CMD ["npm", "start"]
