FROM ubuntu:latest

RUN apt-get update && \
    apt-get install -y curl && \
    apt-get install -y git && \
    git clone https://github.com/docker-hy/backend-example-docker.git


RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && \
    apt-get install -y nodejs

WORKDIR /backend-example-docker

RUN npm install

EXPOSE 8000

CMD ["npm", "start"]

