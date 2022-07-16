FROM node:alpine

# Create app directory
RUN mkdir -p /usr/src/server
WORKDIR /usr/src/server

# Install app dependencies
COPY package.json /usr/src/server/
RUN npm install
# Bundle app source
COPY . /usr/src/server

EXPOSE 3000

CMD [ "npm", "start"]

