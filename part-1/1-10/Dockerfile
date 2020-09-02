FROM ubuntu:latest

RUN apt-get update && \
    apt-get install -y curl && \
    apt-get install -y git && \
    git clone https://github.com/docker-hy/frontend-example-docker.git


RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && \
    apt-get install -y nodejs

WORKDIR /frontend-example-docker

RUN npm install

EXPOSE 5000

CMD ["npm", "start"]

