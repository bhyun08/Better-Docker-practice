FROM centos:7

RUN yum install -y yum-utils && \
    echo -e "[nginx-mainline]\nname=nginx mainline repo\nbaseurl=http://nginx.org/packages/mainline/centos/7/\$basearch/\ngpgcheck=1\nenabled=1\ngpgkey=https://nginx.org/keys/nginx_signing.key" > /etc/yum.repos.d/nginx.repo && \
    yum -y install nginx
