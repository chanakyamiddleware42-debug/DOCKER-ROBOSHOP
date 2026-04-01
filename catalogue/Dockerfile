FROM: node20
workdir  /app
COPY catalogue/package.json .
COPY catalogue/*.js .
RUN npm install 
ENV MONGO="true" \
    MONGO_URL="mongodb://<MONGODB-SERVER-IPADDRESS>:27017/catalogue"
CMD ["node", "server.js"]