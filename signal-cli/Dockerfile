FROM debian:stretch

MAINTAINER redshiftzero <jen@redshiftzero.com>
WORKDIR /opt/signal-cli
RUN apt-get update && apt-get update -y && apt-get install -y default-jre wget
ENV VERSION 0.5.6
RUN wget https://github.com/AsamK/signal-cli/releases/download/v"${VERSION}"/signal-cli-"${VERSION}".tar.gz
RUN tar xf signal-cli-"${VERSION}".tar.gz -C /opt
RUN ln -sf /opt/signal-cli-"${VERSION}"/bin/signal-cli /usr/local/bin/

ENTRYPOINT ["/bin/bash"]
