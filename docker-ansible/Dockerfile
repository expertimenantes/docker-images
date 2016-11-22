FROM ubuntu:14.04
MAINTAINER expertime <arhoussou@expertime.com>
RUN apt-get update && \
    apt-get install --no-install-recommends -y software-properties-common && \
    apt-add-repository ppa:ansible/ansible && \
    apt-get update && \
    apt-get install -y ansible

VOLUME /ansible
WORKDIR /ansible

ENTRYPOINT ["ansible-playbook"]
CMD ["site.yml"]