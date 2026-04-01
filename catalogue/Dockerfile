FROM node:20
WORKDIR /app
COPY catalogue/package.json .
COPY catalogue/*.js .
RUN npm install 
ENV MONGO="true" \
    MONGO_URL="mongodb:mongo:27017/catalogue"
CMD ["node", "server.js"]