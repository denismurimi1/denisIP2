# Creating base image
FROM node:alpine3.18

# setting the working directory
RUN mkdir -p /srv/app/admin-client
WORKDIR /srv/app/admin-client

# Copying the package.json files to the working directory
COPY package*.json /srv/app/admin-client

# Installing the dependencies
RUN npm install --silent
# RUN npm install react-scripts@3.3.1 -g --silent

# Copying the rest of the files to the working directory
COPY . /srv/app/admin-client

# Running the app
CMD ["npm", "start"] 