FROM centos:6

MAINTAINER "Nithesh Mittapally" <nithesh.chandra@gmail.com>

RUN yum -y install wget tar; yum clean all
RUN wget -q --no-check-certificate --no-cookies \
        --header "Cookie: oraclelicense=accept-securebackup-cookie" \
        http://download.oracle.com/otn-pub/java/jdk/7u71-b14/jdk-7u71-linux-x64.rpm \
        -O /var/tmp/jdk-7u71-linux-x64.rpm \
        && rpm -ivh /var/tmp/jdk-7u71-linux-x64.rpm \
        && rm /var/tmp/jdk-7u71-linux-x64.rpm

