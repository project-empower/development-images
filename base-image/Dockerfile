FROM alpine

RUN apk --no-cache add git gnupg openssh-client \
 && mkdir /work \
 && addgroup -g 1000 developer \
 && adduser -D -G developer -u 1000 -h /home/developer developer \
 && chown developer:developer /work

ENV GPG_TTY=/dev/console

USER developer

WORKDIR /work

