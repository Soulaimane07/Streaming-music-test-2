# Use Node.js as the base image
FROM node:20

# Set the working directory
WORKDIR /app

# Copy package.json and package-lock.json from the correct directory
COPY ./frontend/package*.json ./

# Install dependencies
RUN npm install

# Copy the entire app to the container
COPY ./frontend .

# Expose the port that the React app runs on
EXPOSE 3000

# Start the React app
CMD ["npm", "start"]
