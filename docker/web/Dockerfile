FROM ruby:3.2.4

ENV BUNDLER_VERSION=2.5.15

RUN apt-get update -qq && \
  apt-get install -y \
  build-essential \
  libpq-dev \
  nodejs

WORKDIR /app

RUN gem install bundler -v $BUNDLER_VERSION

ENTRYPOINT ["/entrypoint.sh"]