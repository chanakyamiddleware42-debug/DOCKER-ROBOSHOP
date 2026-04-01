FROM node: 20
workdir  /app
COPY catalogue/package.json .
COPY catalogue/*.js .
RUN npm install 
ENV MONGO="true" \
    MONGO_URL="mongodb:mongo:27017/catalogue"
CMD ["node", "server.js"]