FROM node:20

WORKDIR /app

COPY package*.json ./
COPY *.js ./

RUN npm install

ENV CATALOGUE_HOST="catalogue" \
    CATALOGUE_PORT="8080" \
    REDIS_HOST="redis"

CMD ["node", "server.js"]


