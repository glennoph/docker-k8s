# spec base image
FROM node:alpine

WORKDIR /usr/app

# copy package.json file to container
COPY ./package.json ./

# install dependencies
RUN npm install

# copy files to container
COPY ./ ./

# command
CMD ["npm", "start"]

