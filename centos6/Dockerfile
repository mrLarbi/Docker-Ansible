FROM centos:6

# Install dependencies
RUN yum update && \
    yum install -y gcc make python-pip python-devel

RUN pip install ansible cryptography && \
    yum install -y iputils
    
CMD [ "ansible-playbook", "--version" ]
