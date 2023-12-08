FROM ubuntu:latest
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update && apt-get install -y curl kmod
RUN bash -c "bash <(curl -fsSL https://get.docker.com)"
RUN echo "/sbin/modprobe overlay; /usr/bin/containerd & /usr/bin/dockerd --containerd=/run/containerd/containerd.sock &" >> ~/.bash_profile
ENTRYPOINT ["bash", "--login", "-c"]
CMD ["bash"]