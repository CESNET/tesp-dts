FROM ubuntu

ENV DEBIAN_FRONTEND noninteractive
RUN apt update && apt install -y --no-install-recommends \
	nmap \
	s3cmd

ENTRYPOINT ["sleep", "infinity"]

