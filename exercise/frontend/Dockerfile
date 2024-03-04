# Use official Node.js image as the base image
FROM node:latest

# Set working directory
WORKDIR /app/frontend

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the frontend source code
COPY . .

# Expose port 3000
ENV PORT=3000
EXPOSE 3000

# Define the volume
VOLUME [ "/app/frontend" ]

# Command to run the application
CMD ["npm", "start"]
