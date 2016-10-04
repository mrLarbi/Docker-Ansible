FROM debian:jessie

# Install dependencies
RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install build-essential libffi-dev libssl-dev python-pip python-dev -y

RUN pip install ansible cryptography && \
    apt-get install iputils-ping -y

CMD [ "ansible-playbook", "--version" ]
