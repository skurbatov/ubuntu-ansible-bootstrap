# ubuntu-ansible-bootstrap
=======

ubuntu-ansible-bootstrap - ansible playbook to prepare a virtual machine or workstation based on ubuntu.

Requirements
------------

- Link to Ansible role install oh-my-zsh - [ansible-role-oh-my-zsh](git@github.com:gantsign/ansible-role-oh-my-zsh.git)

License
-------

MIT

## Quick Start Guide

### Required dependencies (VirtualBox, Vagrant, Ansible)

  1. Download and install [VirtualBox](https://www.virtualbox.org/wiki/Downloads);
  2. Download and install [Vagrant](http://www.vagrantup.com/downloads.html);
  3. [Mac/Linux only] Install [Ansible](http://docs.ansible.com/intro_installation.html).

### How to local run service
  1. Download this project and put it wherever you want;
  2. Open Terminal, cd to this directory;
  3. Check variables in directory `bootstrap/vagrant.yml`;
  4. Type in `vagrant up`.

## About the Author

This project was created by [Sergey Kurbatov](https://skurbatov.github.io/).