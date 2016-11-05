# Docker-Ansible

[![Build Status](https://travis-ci.org/mrLarbi/Docker-Ansible.svg?branch=master)](https://travis-ci.org/mrLarbi/Docker-Ansible)
[![Ansible Role](https://img.shields.io/badge/docker%20build-automated-blue.svg)](https://hub.docker.com/r/mrlarbi/ansible/)

Docker images with ansible and the networking tools installed.

These images were made for testing purposes.

# Supported Distributions :
    
- CentOS 6
- CentOS 7
- Debian 7 
- Debian 8
- Ubuntu 12.04
- Ubuntu 14.04
- Ubuntu 16.04

# How to use :
    
Pull an image : 

    docker pull mrlarbi/ansible:centos6
    docker pull mrlarbi/ansible:centos7
    docker pull mrlarbi/ansible:debian7 
    docker pull mrlarbi/ansible:debian8 
    docker pull mrlarbi/ansible:ubuntu12.04 
    docker pull mrlarbi/ansible:ubuntu14.04 
    docker pull mrlarbi/ansible:ubuntu16.04 

And then run it :
    
    docker run mrlarbi/ansible:centos6 
    docker run mrlarbi/ansible:centos7 
    docker run mrlarbi/ansible:debian7 
    docker run mrlarbi/ansible:debian8 
    docker run mrlarbi/ansible:ubuntu12.04 
    docker run mrlarbi/ansible:ubuntu14.04 
    docker run mrlarbi/ansible:ubuntu16.04 

Which should display the Ansible version.

# License

GNU General Public License (GPL) V3
