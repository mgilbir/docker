FROM golang:1.7.4

MAINTAINER Miguel Eduardo Gil Biraud <miguel.gil.biraud@ieee.org>

RUN wget http://www.musl-libc.org/releases/musl-1.1.16.tar.gz && \
    tar -xvf musl-1.1.16.tar.gz && \
    cd musl-1.1.16 && \
    ./configure && \
    make && \
    make install && \
    cd .. && rm -rf musl-1.1.16.tar.gz && rm -rf musl-1.1.16 

