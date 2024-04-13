FROM node:14
EXPOSE 8080/tcp
WORKDIR /app
COPY package.json /app
COPY server.js /app
RUN npm install
ENV MONGO=true\
    MONGO_URL="mongodb://mongodb:27017/catalogue"
CMD [ "node", "server.js" ]