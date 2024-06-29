# Use node image as base
FROM node:21

# Set working directory inside the container
WORKDIR /app/frontend

# Copy package.json and package-lock.json (if available) to container
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy all frontend files to container
COPY . .

# Build React app
RUN npm run build

# Expose port 3000 to the outside world
EXPOSE 3000

# Command to run the application
CMD ["npm", "start"]
