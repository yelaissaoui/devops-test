FROM node:8
WORKDIR /usr/src/app
COPY package*.json ./
COPY . .
RUN npm i
RUN npm run build .
CMD ["npm","run","start"]