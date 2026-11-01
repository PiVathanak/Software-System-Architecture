# use node:16-alpine as build
FROM node:22-alpine
# access to the app folder
WORKDIR /app
# copy package.json and package-lock.json
COPY package*.json .
# install dependencies
RUN npm install
# copy the rest of the application code
COPY . .
# set environment variable for the port
ENV PORT=3000
# expose the port
EXPOSE 3000
# run the application
CMD ["npm", "run", "start:dev"]