# Start with a base image containing Node.js runtime
FROM node:14

# Set the working directory in the container
WORKDIR /app

# Add the `package.json` and `package-lock.json` (if available)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of your app's source code
COPY . .

# Make port 3000 available to the world outside this container
EXPOSE 3000

# Build the app
RUN npm run build

# Serve the app using a simple node server
CMD npx serve -s build