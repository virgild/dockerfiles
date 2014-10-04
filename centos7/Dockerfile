FROM centos:centos7
MAINTAINER Virgil Dimaguila "virgild@gmail.com"

ENV REFRESH_DATE "Sep 27 09:27:00 2014"

RUN rpm -ivh http://dl.fedoraproject.org/pub/epel/7/x86_64/e/epel-release-7-2.noarch.rpm
RUN rpm -ivh http://rpms.famillecollet.com/enterprise/remi-release-7.rpm

RUN yum install yum-utils -y
RUN yum-config-manager --enable remi
RUN yum update -y
RUN yum install vim wget bash-completion screen git tar tmux -y
