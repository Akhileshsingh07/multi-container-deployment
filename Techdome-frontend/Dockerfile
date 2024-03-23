#docker pull base image for application from dockerhub
FROM node:21-alpine

#initialize a working directory for container
WORKDIR /app

#copies the package json to Working directory
COPY  package*.json ./

#install all the modules/dependencies of appliaction
RUN npm install

#copy all the files and folders to container Working directory
COPY . .

#post on which we acces our appliaction
EXPOSE 3000

#It runs when conatianer is started
CMD ["npm", "start"]