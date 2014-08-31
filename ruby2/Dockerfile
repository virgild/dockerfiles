FROM virgild/centos6
MAINTAINER Virgil Dimaguila "virgild@gmail.com"

ENV REFRESH_DATE "Sun Aug 24 14:30:27 2014"

RUN yum install gcc make openssl-devel ncurses-devel readline-devel -y
RUN cd /tmp &&  \
  git clone https://github.com/sstephenson/ruby-build.git && \
  cd ruby-build && \
  ./install.sh && \
  ruby-build 2.1.2 /opt/ruby/2.1.2 && \
  rm -rf /tmp/ruby-build*
RUN /opt/ruby/2.1.2/bin/gem install bundler --no-rdoc --no-ri

