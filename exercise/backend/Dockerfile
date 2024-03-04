# Use official Node.js image as the base image
FROM node:latest

# Set working directory
WORKDIR /app/backend

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the backend source code
COPY . .

# Expose port 8000
ENV PORT=8000
EXPOSE 8000

# Define the volume
VOLUME [ "/app/backend" ]

# Command to run the application
CMD ["node", "index.js"]
