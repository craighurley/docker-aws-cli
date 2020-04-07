FROM        python:3.8-alpine3.11
ENV         AWS_PROFILE=default
RUN         apk update \
            && apk add --no-cache groff less \
            && pip3 install --no-cache-dir \
                awscli==1.18.36
WORKDIR     /workdir
ENTRYPOINT  [ "aws" ]
