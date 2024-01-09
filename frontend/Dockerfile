# Use an official Node.js runtime as a parent image
FROM node:16.14
# Set the working directory in the container to /app
WORKDIR /app

# Copy package.json and package-lock.json into the container at /app
COPY package*.json ./

# Install any needed packages specified in package.json
RUN npm install

# Copy the current directory contents into the container at /app
COPY . .

# Make port 5001 available to the world outside this container
EXPOSE 5001

# Run the command to start the SvelteKit server
CMD ["npm", "run", "dev"]