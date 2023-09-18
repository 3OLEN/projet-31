FROM rubylang/ruby:3.2

RUN apt-get update  \
    && apt-get install -y \
        gcc \
        g++ \
        make

RUN gem install minimal jekyll bundler

WORKDIR /app/docs

COPY entrypoint /entrypoint
ENTRYPOINT ["/entrypoint"]
