# Version: 0.0.1
FROM ubuntu:15.10
MAINTAINER dj_xc "dj_xc@163.com"
RUN mv /etc/apt/sources.list /etc/apt/sources.list.bak && \
    echo "deb-src http://archive.ubuntu.com/ubuntu xenial main restricted" >/etc/apt/sources.list && \
    echo "deb http://mirrors.aliyun.com/ubuntu/ xenial main restricted" >>/etc/apt/sources.list && \
    echo "deb-src http://mirrors.aliyun.com/ubuntu/ xenial main restricted multiverse universe" >>/etc/apt/sources.list && \
    echo "deb http://mirrors.aliyun.com/ubuntu/ xenial-updates main restricted" >>/etc/apt/sources.list && \
    echo "deb-src http://mirrors.aliyun.com/ubuntu/ xenial-updates main restricted multiverse universe" >>/etc/apt/sources.list && \
    echo "deb http://mirrors.aliyun.com/ubuntu/ xenial universe" >>/etc/apt/sources.list && \
    echo "deb http://mirrors.aliyun.com/ubuntu/ xenial-updates universe" >>/etc/apt/sources.list && \
    echo "deb http://mirrors.aliyun.com/ubuntu/ xenial multiverse" >>/etc/apt/sources.list && \
    echo "deb http://mirrors.aliyun.com/ubuntu/ xenial-updates multiverse" >>/etc/apt/sources.list && \
    echo "deb http://mirrors.aliyun.com/ubuntu/ xenial-backports main restricted universe multiverse" >>/etc/apt/sources.list && \
    echo "deb-src http://mirrors.aliyun.com/ubuntu/ xenial-backports main restricted universe multiverse" >>/etc/apt/sources.list && \
    echo "deb http://archive.canonical.com/ubuntu xenial partner" >>/etc/apt/sources.list && \
    echo "deb-src http://archive.canonical.com/ubuntu xenial partner" >>/etc/apt/sources.list && \
    echo "deb http://mirrors.aliyun.com/ubuntu/ xenial-security main restricted" >>/etc/apt/sources.list && \
    echo "deb-src http://mirrors.aliyun.com/ubuntu/ xenial-security main restricted multiverse universe" >>/etc/apt/sources.list && \
    echo "deb http://mirrors.aliyun.com/ubuntu/ xenial-security universe" >>/etc/apt/sources.list && \
    echo "deb http://mirrors.aliyun.com/ubuntu/ xenial-security multiverse" >>/etc/apt/sources.list
RUN apt-get update
RUN apt-get install -y nginx
RUN echo 'Hi, I am in your container' > /usr/share/nginx/html/index.html
EXPOSE 80
