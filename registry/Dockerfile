#Dockerfile
FROM centos-base6
MAINTAINER minghui.zhang <minghui.zhang@163.com>
RUN yum -y install docker-registry
RUN echo -e "#!/bin/sh\nservice docker-registry start\n/usr/sbin/sshd -D">/etc/init.d/apps.sh
RUN chmod u+x /etc/init.d/apps.sh
CMD /etc/init.d/apps.sh

