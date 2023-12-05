# Use an official Node runtime as a parent image
FROM node:16.15.0

# Set the working directory in the container
WORKDIR /niti_chatbot/niti-client

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install dependencies
RUN npm install

# Bundle your app's source code inside the Docker image
COPY . .


# Expose port 3000 to the outside world
EXPOSE 3000

# Start the application
CMD ["npm", "start"]