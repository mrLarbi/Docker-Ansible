FROM centos:7

# Install dependencies
RUN yum update -y && \
    yum install -y epel-release \
    yum install -y gcc make python-pip python-devel

RUN pip install ansible cryptography && \
    yum install -y iputils
    
CMD [ "ansible-playbook", "--version" ]
