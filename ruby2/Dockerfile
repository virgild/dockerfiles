FROM virgild/centos7
MAINTAINER Virgil Dimaguila "virgild@gmail.com"

RUN yum install gcc make openssl-devel ncurses-devel readline-devel -y
RUN cd /tmp &&  \
  git clone https://github.com/sstephenson/ruby-build.git && \
  cd ruby-build && \
  ./install.sh && \
  ruby-build 2.1.3 /opt/ruby/2.1.3 && \
  rm -rf /tmp/ruby-build*
RUN /opt/ruby/2.1.3/bin/gem install bundler --no-rdoc --no-ri

