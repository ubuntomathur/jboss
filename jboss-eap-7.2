FROM centos:7
RUN yum update -y && \
   yum install -y --setopt=tsflags=nodocs augeas  bsdtar iputils java-1.8.0-openjdk-devel less \
   net-tools nmap-ncat  procps-ng tar traceroute unzip xmlstarlet \
   && yum clean all
RUN groupadd -r jboss -g 1000 \
    && useradd -u 1000 -r -g jboss -m -d /opt/jboss -s /sbin/nologin -c "JBoss user" jboss  \
    && chmod 755 /opt/jboss
WORKDIR /opt/jboss
USER jboss
ENV JBOSS_HOME /opt/jboss/jboss-eap-7.2
ADD jboss-eap-7.2.0.zip  /opt/jboss
RUN  unzip jboss-eap-7.2.0.zip
RUN $JBOSS_HOME/bin/add-user.sh admin jboss#1! --silent
EXPOSE 8080 9990
CMD ["/opt/jboss/jboss-eap-7.2/bin/standalone.sh", "-b", "0.0.0.0", "-bmanagement", "0.0.0.0"]
