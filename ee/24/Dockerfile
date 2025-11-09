FROM container-registry.oracle.com/graalvm/jdk:24-ol9

LABEL author="faiz"

RUN useradd -d /home/container -m container

USER container
ENV USER=container HOME=/home/container
WORKDIR /home/container

COPY ../../entrypoint.sh /entrypoint.sh
CMD [ "/bin/bash", "/entrypoint.sh" ]
