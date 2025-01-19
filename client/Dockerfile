FROM node:lts-slim
WORKDIR /usr/src/app

COPY package.json /usr/src/app
# COPY package-lock.json /usr/src/app
RUN npm install  --legacy-peer-deps
#RUN npm ci


COPY . /usr/src/app
# Expose the port the app runs in
EXPOSE 3000

CMD [ "npm", "run", "start"]
