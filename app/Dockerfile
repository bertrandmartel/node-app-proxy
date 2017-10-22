
FROM node:latest

MAINTAINER Bertrand Martel <bmartel.fr@gmail.com>

# Create app directory
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

# Install app dependencies
COPY package.json /usr/src/app/
RUN npm install

COPY app.js /usr/src/app/
COPY index.html /usr/src/app/

ADD start.sh /var/www/
RUN chmod +x /var/www/start.sh

CMD ["/var/www/start.sh"] 
