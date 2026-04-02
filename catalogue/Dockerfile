FROM node:20
WORKDIR /app
COPY catalogue/package.json .
COPY catalogue/*.js .
RUN npm install 
ENV MONGO="true"\
    MONGO_URL="mongodb://mongodb:27017/catalogue"
#Environment=MONGO_URL="mongodb://<MONGODB-SERVER-IPADDRESS>:27017/catalogue"
CMD ["node", "server.js"]