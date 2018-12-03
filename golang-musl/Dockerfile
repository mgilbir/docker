FROM golang:1.11.2

MAINTAINER Miguel Eduardo Gil Biraud <miguel.gil.biraud@ieee.org>

RUN wget http://www.musl-libc.org/releases/musl-1.1.20.tar.gz && \
    tar -xvf musl-1.1.20.tar.gz && \
    cd musl-1.1.20 && \
    ./configure && \
    make && \
    make install && \
    cd .. && rm -rf musl-1.1.20.tar.gz && rm -rf musl-1.1.20 

