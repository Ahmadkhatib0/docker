FROM node:14

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 80

# VOLUME ["/app/feedback"]

# CMD [ "node", "server.js" ]
CMD [ "npm", "start" ]
# to use nodemon instead to what for changes in js files 