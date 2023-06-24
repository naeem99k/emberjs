# Use the official Node.js 14 image.
# More info about this image: https://hub.docker.com/_/node
FROM node:20

# Set the working directory
WORKDIR /usr/src/app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install all dependencies
RUN npm install

# Install Ember CLI globally
RUN npm install -g ember-cli

# Copy all files
COPY . .

# Expose the port the app runs in
EXPOSE 4200

# Serve the app
CMD ["ember", "serve"]