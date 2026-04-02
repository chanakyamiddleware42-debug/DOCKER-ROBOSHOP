FROM node:20
WORKDIR /app
COPY cart-v3/package.json .
COPY cart-v3/*.js .
RUN npm install 
ENV REDIS_HOST="redis"\
    CATALOGUE_HOST="catalogue"\
    CATALOGUE_PORT="8080"
#Environment=MONGO_URL="mongodb://mongodb:27017/users"
CMD ["node", "server.js"]