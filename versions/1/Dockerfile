FROM        python:3.8-alpine3.11
ENV         AWS_PROFILE=default
COPY        docker-entrypoint.sh /usr/local/bin/
RUN         chmod +x /usr/local/bin/docker-entrypoint.sh \
            && pip3 install --no-cache-dir \
                awscli==1.18.36
WORKDIR     /workdir
ENTRYPOINT  [ "aws" ]
