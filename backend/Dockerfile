# Use Node.js 20 LTS as the base image
FROM node:20-alpine

# Set working directory
WORKDIR /app

# Copy package files first
COPY package*.json ./

# Install dependencies
RUN npm ci

# Copy the application source code
COPY . .

# Expose the backend port
EXPOSE 5000

# Start the backend server
CMD ["node", "src/server.js"]
