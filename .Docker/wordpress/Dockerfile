ARG WORDPRESS_VERSION

FROM ${WORDPRESS_VERSION}

RUN set -eux \
  && apt-get -y update \
  && apt-get -y upgrade \
  && apt-get install -y vim \
  && apt-get install -y locales \
  && rm -rf /var/lib/apt/lists/* \
  && echo "ja_JP.UTF-8 UTF-8" > /etc/locale.gen \
  && locale-gen ja_JP.UTF-8

ENV LANG ja_JP.UTF-8

WORKDIR /var/www/html