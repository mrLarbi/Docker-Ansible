FROM ubuntu:14.04

# Install dependencies
RUN apt-get update && \
    apt-get upgrade && \
    apt-get install build-essential libffi-dev libssl-dev python-pip python-dev -y

RUN pip install ansible && \
    apt-get install iputils-ping

CMD [ "ansible-playbook", "--version" ]
