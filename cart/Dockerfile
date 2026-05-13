FROM node:20
WORKDIR /app
COPY package.json .
COPY *.js .
RUN npm install
ENV REDIS_HOST="redis" \
    CATALOGUE_HOST="catalogue" \
    REDIES_URL="redis://redis:6379" \
    CATALOGUE_PORT="80"
CMD ["node","server.js"]