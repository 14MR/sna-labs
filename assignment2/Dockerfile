FROM alpine:3.10
MAINTAINER Timur Mustafin <t.mustafin@innopolis.ru>

RUN apk --update add --no-cache openssh \
  && echo "root:root" | chpasswd \
  && rm -rf /var/cache/apk/*

RUN /usr/bin/ssh-keygen -A # generate keys if they do not exist

EXPOSE 22

CMD ["/usr/sbin/sshd","-D"]
