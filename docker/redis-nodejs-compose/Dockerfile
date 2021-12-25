FROM node:alpine

# set workdir
WORKDIR '/app'

# dependencies
COPY package.json .
RUN npm install

# copy files to workdir
COPY . .

# start npm
CMD ["npm", "start"]

