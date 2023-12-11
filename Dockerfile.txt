FROM node:14
WORKDIR /usr/src/app
COPY package*.json server.js ./
RUN npm install
RUN npm install express
# COPY . .
# COPY server.js ./
EXPOSE 3000
CMD ["node", "server.js"]
