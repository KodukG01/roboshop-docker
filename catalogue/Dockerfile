FROM node:20-alpine3.21
WORKDIR /opt/server
COPY package.json .
COPY *.js .
RUN npm install
ENV MONGO="true" \
    MONGO_URL="mongodb://mongodb:27017" 
CMD ["node", "server.js"]