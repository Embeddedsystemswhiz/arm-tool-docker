FROM debian:latest
LABEL maintainer="kayasdev@gmail.com"
ARG DEBIAN_FRONTEND=noninteractive

RUN apt-get update && \
    DEBIAN_FRONTEND=noninteractive apt-get -qq install \
    wget \ 
    cmake \
    tar \
    libncurses-dev \
    xz-utils 


## Linux 64bit
RUN wget https://developer.arm.com/-/media/Files/downloads/gnu/11.2-2022.02/binrel/gcc-arm-11.2-2022.02-x86_64-aarch64-none-linux-gnu.tar.xz && \
   tar xf gcc-arm-11.2-2022.02-x86_64-aarch64-none-linux-gnu.tar.xz -C /opt/ 
ENV PATH="/opt/gcc-arm-11.2-2022.02-x86_64-aarch64-none-linux-gnu/bin:${PATH}"
