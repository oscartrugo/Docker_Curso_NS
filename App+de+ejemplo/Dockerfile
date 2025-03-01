FROM node:20.5.0-alpine3.18
WORKDIR /app/
COPY package*.json .
RUN npm install
COPY . .
# privnenv API para imprimir la variable de entorno
ENV API=https://apiv1.miweb.com
