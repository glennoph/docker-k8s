# spec base image
FROM node:alpine

WORKDIR /usr/app

# copy files to container
COPY ./ ./

# install dependencies
RUN npm install

# command
CMD ["npm", "start"]

