FROM ubuntu:16.04
MAINTAINER wufeigui@foxmail.com
WORKDIR /root
COPY sources.list /etc/apt/sources.list.d/alibaba.list
RUN  apt-get update 
RUN  apt-get install libc-bin debconf locales -y \
	&& apt-get install -y language-pack-zh-hans \
	&& echo "export LC_ALL=zh_CN.UTF-8">> /etc/profile
ENV LC_ALL=zh_CN.utf8
RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime
