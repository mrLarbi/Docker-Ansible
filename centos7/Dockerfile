FROM centos:7

# Install dependencies
RUN yum update -y && \
    yum install -y epel-release && \
    yum install -y gcc make libffi-devel openssl-devel python-pip python-devel

#Upgrade pip
RUN pip install --upgrade pip

#Install Ansible and the networking tools
RUN pip install ansible cryptography && \
    yum install -y iputils iproute


#Activate systemd
ENV container=docker
RUN (cd /lib/systemd/system/sysinit.target.wants/; for i in *; do [ $i == systemd-tmpfiles-setup.service ] || rm -f $i; done); \
    rm -f /lib/systemd/system/multi-user.target.wants/*;\
    rm -f /etc/systemd/system/*.wants/*;\
    rm -f /lib/systemd/system/local-fs.target.wants/*; \
    rm -f /lib/systemd/system/sockets.target.wants/*udev*; \
    rm -f /lib/systemd/system/sockets.target.wants/*initctl*; \
    rm -f /lib/systemd/system/basic.target.wants/*;\
    rm -f /lib/systemd/system/anaconda.target.wants/*;
VOLUME ["/sys/fs/cgroup"]

#Default command    
CMD [ "ansible-playbook", "--version" ]
