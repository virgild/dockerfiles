FROM centos:centos6
MAINTAINER Virgil Dimaguila "virgild@gmail.com"

ENV REFRESH_DATE "Tue Aug 19 08:41:00 2014"

RUN rpm -ivh http://dl.fedoraproject.org/pub/epel/6/x86_64/epel-release-6-8.noarch.rpm
RUN rpm -ivh http://rpms.famillecollet.com/enterprise/remi-release-6.rpm
RUN rpm -ivh http://yum.puppetlabs.com/puppetlabs-release-el-6.noarch.rpm

RUN yum install yum-utils -y
RUN yum-config-manager --enable remi
RUN yum update -y
RUN yum install puppet vim wget bash-completion screen git tar tmux -y
