# Use node image as base
FROM node:21

# Set working directory inside the container
WORKDIR /app/server

# Copy package.json and package-lock.json (if available) to container
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy all server files to container
COPY . .

# Expose port 4000 to the outside world
EXPOSE 4000

# Command to run the server using nodemon for hot reload
CMD ["npm", "run", "dev"]
