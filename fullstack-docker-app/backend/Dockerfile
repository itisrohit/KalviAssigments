# Use Node base image
FROM node:14-alpine

# Set working directory inside container
WORKDIR /usr/src/app

# Copy package files and install dependencies
COPY package*.json ./
RUN npm install

# Copy the rest of the code
COPY . .

# Expose port for backend
EXPOSE 5000

# Start the backend server
CMD ["npm", "start"]