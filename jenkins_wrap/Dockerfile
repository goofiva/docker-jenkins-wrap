FROM jenkins
COPY plugins.txt /plugins.txt
USER root
RUN apt-get install git
USER jenkins
RUN /usr/local/bin/plugins.sh /plugins.txt