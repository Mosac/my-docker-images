FROM library/ruby:2.6.3-alpine3.9
LABEL maintainer="Mosac https://github.com/Mosac"

RUN apk update && \
    apk upgrade && \
    apk add --update --no-cache --virtual=.build-dependencies \
      bash \
      build-base \
      curl \
      curl-dev \
      pcre \
      nodejs \
      libstdc++ \
      libxml2-dev \
      libxslt-dev \
      linux-headers \
      libxml2-dev \
      libxslt-dev \
      postgresql-dev \
      mysql-client \
      mysql-dev \
      sqlite-dev \
      ruby-dev \
      ruby-json \
      tzdata \
      yaml \
      yaml-dev \
      zlib-dev && \
    apk add --update --no-cache \
      bash \
      git \
      openssh \
      postgresql \
      ruby-json \
      tzdata \
      yaml && \
    apk del .build-dependencies

WORKDIR /app

ENTRYPOINT [ "/bin/bash" ]
