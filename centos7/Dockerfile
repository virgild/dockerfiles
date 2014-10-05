FROM centos:centos7
MAINTAINER Virgil Dimaguila "virgild@gmail.com"

RUN rpm -ivh http://dl.fedoraproject.org/pub/epel/7/x86_64/e/epel-release-7-2.noarch.rpm
RUN rpm -ivh http://rpms.famillecollet.com/enterprise/remi-release-7.rpm

RUN yum install yum-utils hostname -y
RUN yum-config-manager --enable remi
RUN yum update -y
