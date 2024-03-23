# Docker image as the base image
FROM mongo:latest

# Set the working directory within the container
WORKDIR /usr/src/app

# Copy the package.json file to the container working directory
COPY package.json .

# Install dependencies
RUN npm install

# Copy the application code to the container
COPY . .

# port on which this container runs
EXPOSE 27017

# Command run container starts
CMD ["node", "start"]



