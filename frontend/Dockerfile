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

# Expose the Next.js port
EXPOSE 3000

# Start the frontend application
CMD ["npm", "run", "dev"]
