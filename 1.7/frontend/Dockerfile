FROM ubuntu:16.04

WORKDIR /1.5
COPY /frontend-example-docker .
RUN apt-get update -y && apt-get install curl -y
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN npm install
EXPOSE 5000
CMD API_URL=http://localhost:8000 npm start
