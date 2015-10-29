FROM jenkins
COPY plugins.txt /plugins.txt
USER root
RUN apt-get update
RUN apt-get install git -y
RUN apt-get install software-properties-common -y
RUN add-apt-repository ppa:cwchien/gradle \
  && apt-get update \
  && apt-get install gradle -y
USER jenkins
RUN /usr/local/bin/plugins.sh /plugins.txt