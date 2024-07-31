# Use the official Node.js image.
# The tag '18-alpine' is a smaller version of Node.js based on Alpine Linux.
# Replace with the appropriate version based on your needs.
FROM node:18-alpine

# Set the working directory in the container.
WORKDIR /usr/src/app

# Copy package.json and package-lock.json first to leverage Docker cache.
# This step ensures that dependencies are cached unless package.json changes.
COPY package*.json ./

# Install app dependencies.
RUN npm install

# Copy the rest of your application code to the container.
COPY src/ .

# Build the application if needed (e.g., for TypeScript projects).
# RUN npm run build

# Expose the port your app will run on.
EXPOSE 3000

# Command to run your app using Node.js.
CMD ["npm", "start"]
