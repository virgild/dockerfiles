FROM virgild/ruby2
MAINTAINER Virgil Dimaguila "virgild@gmail.com"

ENV REFRESH_DATE "Thu Aug 28 20:43:56 2014"

RUN yum install gcc-c++ curl-devel pcre-devel -y
RUN /opt/ruby/2.1.3/bin/gem install passenger --no-rdoc --no-ri
RUN /opt/ruby/2.1.3/bin/passenger-install-nginx-module --auto --auto-download --prefix=/opt/nginx --extra-configure-flags="--with-http_ssl_module" --languages ruby
