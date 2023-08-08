# Requires node:18-alpine as the base image for Dockerizing the Node.js application
FROM node:18-alpine
# Creating the working directory
WORKDIR /app
# Copying the dependencies in the package.json file
COPY package.json .
COPY yarn.lock .
#Installing all the dependencies
RUN yarn
#Copying all the files to the working directory
COPY . .
#Container will run on this port
EXPOSE 4000
#Command to start the Docker container Node.js application
CMD ["npm", "run", "start"]
