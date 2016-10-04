FROM ubuntu:12.04

# Install dependencies
RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install build-essential libffi-dev libssl-dev python-pip python-dev -y

RUN pip install ansible && \
    apt-get install iputils-ping -y

CMD [ "ansible-playbook", "--version" ]
