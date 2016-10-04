FROM centos:6

# Install dependencies
RUN yum update && \
    yum install gcc make python-pip python-devel -y

RUN pip install ansible cryptography && \
    yum install iputils
    
CMD [ "ansible-playbook", "--version" ]
