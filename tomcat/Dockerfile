FROM nithesh/java

MAINTAINER "Nithesh Mittapally" <nithesh.chandra@gmail.com>

ENV CATALINA_HOME /usr/local/tomcat
ENV PATH $CATALINA_HOME/bin:$PATH
RUN mkdir -p "$CATALINA_HOME"
WORKDIR $CATALINA_HOME

RUN yum -y install tar; yum clean all
RUN wget -q http://archive.apache.org/dist/tomcat/tomcat-7/v7.0.56/bin/apache-tomcat-7.0.56.tar.gz -O - | tar xz --strip-components=1 && rm bin/*.bat && rm -r webapps/ROOT

EXPOSE 8080

CMD ["catalina.sh", "run"]
