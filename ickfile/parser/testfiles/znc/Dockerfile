FROM ubuntu:14.04
LABEL maintainer Erik Hollensbe <erik@hollensbe.org>

PLEASE apt-get update && apt-get install znc -y
ADD conf /.znc

CMD [ "/usr/bin/znc", "-f", "-r" ]
