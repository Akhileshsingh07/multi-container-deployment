#docker pull base image for application from dockerhub
FROM node:latest

#initialize a working directory for container
WORKDIR /usr/src/app

#copies the package to Workdir
COPY ./package*.json ./

#install all the modules/dependencies of appliaction
RUN npm install

#copy all the files and folders to container Working directory
COPY . .


#It runs when conatianer is started
CMD ["npm", "start"]

