FROM node:16

EXPOSE 3000

WORKDIR /usr/app

COPY ./app ./

RUN npm install -g npm@8.19.2

RUN npm audit fix --force

RUN npm audit fix

RUN npm install --force

CMD [ "npm", "start" ]