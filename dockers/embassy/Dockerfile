#
#   Author: Rohith (gambol99@gmail.com)
#   Date: 2014-11-24 14:38:29 +0000 (Mon, 24 Nov 2014)
#
#  vim:ts=2:sw=2:et
#
FROM centos
MAINTAINER <gambol99@gmail.com>

ADD ./stage/startup.sh ./startup.sh
RUN curl -ksL https://github.com/gambol99/embassy/releases/download/v0.0.3-hfx.0/embassy-v0.0.3-hfx.0 -o /bin/embassy
RUN chmod +x /startup.sh; chmod +x /bin/embassy
ENTRYPOINT [ "/startup.sh" ]
