FROM node:7.7.2-alpine

RUN mkdir -p /home/node/app/node_modules && chown -R node:node /home/node/app

WORKDIR /usr/app

COPY package*.json ./

RUN npm install --quiet

COPY --chown=node:node . .

CMD [ "npm", "start" ]