FROM node:alpine
WORKDIR /app
ENV MONGO_DB_USERNAME=root \
    MONGO_DB_PWD=password
COPY package.json .
RUN npm install
COPY . .
EXPOSE 3000
CMD [ "node", "server.js" ]