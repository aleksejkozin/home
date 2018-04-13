FROM debian:latest

RUN apt-get update \
    && apt-get install -y \
        build-essential \
        curl \
    && curl -L https://www.inet.no/dante/files/dante-1.4.2.tar.gz | tar xz \
    && cd dante-* \
    && ./configure \
    && make -j \
    && make install
