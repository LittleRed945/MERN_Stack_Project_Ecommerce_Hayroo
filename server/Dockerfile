FROM node:lts-slim
WORKDIR /usr/src/app

COPY package.json /usr/src/app
# COPY package-lock.json /usr/src/app
RUN npm install
#RUN npm ci

COPY . /usr/src/app
# Expose the port the app runs in
EXPOSE 8000

CMD [ "npm", "run", "start:dev"]