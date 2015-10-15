FROM centos:centos5
MAINTAINER tcnksm "nsd22843@gmail.com"

RUN yum -y update && yum -y groupinstall 'Development Tools' && yum -y install \
    kernel-devel \
    ImageMagick-devel \
    bzip2-devel \
    libcurl \
    libcurl-devel \
    openssl-devel \
    libevent-devel \
    libffi-devel \
    glib2-devel \
    libjpeg-devel \
    mysql-devel \
    postgresql-devel \
    ncurses-devel \
    readline \
    readline-devel \
    sqlite-devel \
    openssl \
    openssl-devel \
    libxml2-devel \
    libxslt-devel \
    zlib-devel \
    wget \
    && yum clean all

RUN rpm --import http://dl.fedoraproject.org/pub/epel/RPM-GPG-KEY-EPEL-5 \
    && rpm -Uvh http://dl.fedoraproject.org/pub/epel/5/x86_64/epel-release-5-4.noarch.rpm \
    && yum -y install libyaml-devel \
    && yum clean all

RUN yum -y update && yum install -y \
    bzr \
    mercurial \
    && yum clean all

RUN yum -y update && yum install -y \
    tar \
    && yum clean all
