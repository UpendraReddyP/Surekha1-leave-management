# Use Node.js base image
FROM node:18

# Set working directory
WORKDIR /app

# Copy package files and install dependencies
COPY package*.json ./
RUN npm install

# Copy the rest of the code
COPY . .

# Create upload directory
RUN mkdir -p uploads

# Expose backend port
EXPOSE 3020

# Start the server
CMD ["node", "server.js"]

