# Use an official Node runtime as a parent image
FROM node:latest

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy the current directory contents into the container at /usr/src/app
COPY . .

# Install any needed packages specified in package.json
RUN npm install

# Build the SvelteKit app
RUN npm run build

# Make port 3000 available to the world outside this container
EXPOSE 3000

# Run npm run preview when the container launches
CMD ["npm", "run", "preview"]
