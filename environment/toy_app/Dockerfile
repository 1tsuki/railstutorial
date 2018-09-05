FROM ruby:2.5
RUN apt-get update -qq && apt-get install -y build-essential libpq-dev nodejs
RUN mkdir /toy_app
WORKDIR /toy_app
COPY Gemfile /toy_app/Gemfile
COPY Gemfile.lock /toy_app/Gemfile.lock
RUN bundle install
COPY . /toy_app