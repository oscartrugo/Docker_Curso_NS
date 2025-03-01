FROM node:20.5.0-alpine3.18
RUN addgroup react && adduser -S -G react react
USER react
WORKDIR /app/
COPY --chown=react package*.json .
RUN npm install
COPY --chown=react . .
# privnenv API para imprimir la variable de entorno
ENV API=https://apiv1.miweb.com
# Expone el puerto que se utiliza (informativo, no determina el valor)
EXPOSE 5173
# Ejecutamos el comando para iniciar la app de React
CMD [ "npm", "run", "dev" ]