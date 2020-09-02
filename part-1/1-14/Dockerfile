FROM ruby:2.6.0

RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && \
    apt-get install -y nodejs && \
    git clone https://github.com/docker-hy/rails-example-project.git

WORKDIR rails-example-project

RUN bundle install && \
    rails db:migrate

EXPOSE 3000:3000

CMD rails s

