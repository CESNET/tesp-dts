FROM ubuntu

ENV DEBIAN_FRONTEND noninteractive
RUN apt update && apt install -y --no-install-recommends \
        curl \
        wget \
        nmap \
        vim \
        s3cmd

COPY .s3cfg /root/

ENTRYPOINT ["sleep", "infinity"]

