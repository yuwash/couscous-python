FROM composer/composer:alpine

LABEL maintainer "Yushin Washio <yuwash at yandex dot com>"

RUN composer global require couscous/couscous
RUN set -x \
        && apk add --no-cache \
                python3 \
        && cd $(dirname $(which python3)) \
                && ln -s python3 python

WORKDIR /project
EXPOSE 8000
ENTRYPOINT ["couscous"]
