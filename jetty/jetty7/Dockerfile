FROM xetius/jdk:8
MAINTAINER Chris Hudson <chris@xetius.com>

ENV JETTY_VERSION 7.6.3.v20120416
ENV JETTY_DOWNLOAD http://central.maven.org/maven2/org/eclipse/jetty/jetty-distribution/${JETTY_VERSION}/jetty-distribution-${JETTY_VERSION}.tar.gz
ENV JETTY_HOME /usr/share/jetty

RUN curl ${JETTY_DOWNLOAD} | tar -xz
RUN mv jetty-distribution-${JETTY_VERSION} ${JETTY_HOME}

WORKDIR ${JETTY_HOME}

ENTRYPOINT ["java", "-jar", "start.jar"]

