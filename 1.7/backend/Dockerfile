FROM ubuntu:16.04

WORKDIR /1.6
COPY /backend-example-docker .
RUN apt-get update -y && apt-get install curl -y
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN npm install
EXPOSE 8000
CMD FRONT_URL=http://localhost:5000 npm start

