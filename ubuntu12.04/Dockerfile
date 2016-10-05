FROM ubuntu:12.04

# Install dependencies
RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install build-essential libffi-dev libssl-dev python-pip python-dev -y

#Upgrade pip
RUN pip install --upgrade pip

#Install Ansible and the networking tools
RUN pip install ansible cryptography && \
    apt-get install iputils-ping -y

#Default command
CMD [ "ansible-playbook", "--version" ]
