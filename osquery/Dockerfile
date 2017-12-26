FROM ubuntu:16.04
MAINTAINER redshiftzero <jen@redshiftzero.com>
RUN apt-get update && apt-get upgrade -y && \
    apt-get install -y apt-transport-https software-properties-common
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 1484120AC4E9F8A1A577AEEE97A80C63C9D8B80B
RUN add-apt-repository "deb [arch=amd64] https://osquery-packages.s3.amazonaws.com/xenial xenial main"
RUN apt-get update && apt-get upgrade -y && apt-get install -y osquery
CMD ["/usr/bin/osqueryi"]
