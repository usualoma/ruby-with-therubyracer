FROM ruby:2.4.1-slim

RUN set -ex \
  \
  && apt-get update \
  && apt-get -y install g++ make \
  && gem install therubyracer \
  && rm -fr $(dirname $(dirname $(gem which libv8)))/vendor \
  && apt-get -y autoremove --purge g++ make \
  && apt-get clean \
  && rm -rf /var/cache/apt/archives/* /var/lib/apt/lists/*
