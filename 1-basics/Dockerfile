FROM node

WORKDIR /app 
# this because we'll host our project in the app folder of the container
# so we wanna till docker to run such commands (eg npm install) inside 
# this app folder, because it run them inside the root folder by default

COPY . /app
# copy * in this project to /app in the container system file
# COPY . ./ 
# the tow commands are the same, because we've specified WORKDIR above

RUN npm install
# run runs during the build time,so its not correct to say 
# RUN node server.js , instead CMD runs after the image has been built 

EXPOSE 80

CMD ["node" , "server.js"] 
# if you don't specify a CMD , the (CMD of the base image) will be excited
# with no base image and no CMD, you'd get an error 
