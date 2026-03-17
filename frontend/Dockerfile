FROM node:21-alpine3.17

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

ARG REACT_APP_API_BASE_UR
ENV REACT_APP_API_BASE_UR=$REACT_APP_API_BASE_UR

RUN npm run build

CMD [ "npx","server","-s","build","-l","3000" ]