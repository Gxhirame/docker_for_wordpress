ARG MYSQL_VERSION

FROM ${MYSQL_VERSION}

RUN set -eux \
  && apt-get update \
  && apt-get -y upgrade \
  && apt-get install -y vim \
  && apt-get install -y locales \
  && rm -rf /var/lib/apt/lists/* \
  && echo "ja_JP.UTF-8 UTF-8" > /etc/locale.gen \
  && locale-gen ja_JP.UTF-8

ENV LANG ja_JP.UTF-8