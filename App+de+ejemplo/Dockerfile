FROM node:20.5.0-alpine3.18
WORKDIR /app/
COPY package*.json .
RUN npm install
COPY . .
# privnenv API para imprimir la variable de entorno
ENV API=https://apiv1.miweb.com
# Expone el puerto que se utiliza (informativo, no determina el valor)
EXPOSE 5173
# Ejecutamos el comando para iniciar la app de React
CMD [ "npm", "run", "dev" ]