FROM node:latest
RUN mkdir -p /usr/src/appo
# Create app directory
WORKDIR /usr/src/appo

# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)

COPY package*.json ./

RUN npm install
# If you are building your code for production
# RUN npm ci --only=production

# Bundle app source
COPY . /usr/src/appo

EXPOSE 3000
CMD [ "npm", "start" ]