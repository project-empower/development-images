FROM alpine

RUN apk add git
RUN mkdir /work
RUN addgroup -g 1000 developer
RUN adduser -D -G developer -u 1000 -h /home/developer developer

RUN chown developer:developer /work

RUN apk add gnupg
RUN apk add openssh-client

ENV GPG_TTY=/dev/console

USER developer

WORKDIR /work

