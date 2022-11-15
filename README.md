# Project 11: ANSIBLE CONFIGURATION MANAGEMENT AUTOMATE PROJECT 7 TO 10.

## Table of Contents
- [Introduction](#introduction)
- [Install and configure Ansible on an EC2 instance](#install-and-configure-ansible-on-an-ec2-instance)


## Introduction
In this project, we would be configuring Ansible Client as a Bastion Host also known as Jump Server. A Jump server is an intermediary server through which access to the internal network can be provided. If we should consider the current architecture being worked on, the web servers are always inside a secure network that cannot be reached directly from the internet. This means that even a DevOps engineer cannot ssh into the web servers directly except through a Jump server, this provides better security and reduces attack surface.

In the diagram shown below the Virtual Private Network is divided into two subnets:
- Public subnet: This has public IP addresses and is accessible from the internet.
- Private subnet: This is only reachable by private IP addresses and is not accessible from the internet.

![alt text](https://darey.io/wp-content/uploads/2021/07/bastion.png)

In this project, we would develop Ansible scripts to simulate the use of a Jump Box to access our Web Servers.


## Install and configure Ansible on an EC2 instance