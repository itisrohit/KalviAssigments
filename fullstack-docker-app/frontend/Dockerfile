# Use Node base image
FROM node:14-alpine

# Set working directory inside container
WORKDIR /usr/src/app

# Copy package files and install dependencies
COPY package*.json ./
RUN npm install

# Copy the rest of the frontend code
COPY . .

# Expose port for React dev server
EXPOSE 3000

# Start the React app
CMD ["npm", "start"]