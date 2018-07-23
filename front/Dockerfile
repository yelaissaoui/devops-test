FROM node:8
WORKDIR /usr/src/app
COPY package*.json ./
COPY . .
npm i
npm build .
EXPOSE 80
CMD ["npm","start"]