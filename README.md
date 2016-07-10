# Ansible Role: Beetbox Silverstripe

[![CircleCI](https://circleci.com/gh/beetboxvm/ansible-role-beetbox-silverstripe.svg?style=svg)](https://circleci.com/gh/beetboxvm/ansible-role-beetbox-silverstripe)

An Ansible role that creates and installs a Silverstripe project on beetbox.

## Requirements

This role is specifically developed as an extension to beetbox -- https://github.com/beetboxvm/beetbox

## Role Variables

Available variables are listed below, along with default values:

Create a new Silverstripe project.

    ss_create_project: no
    
Silverstripe project version. Composer compatible version, leave blank to use the latest version.
    
    ss_version: ""
    
Install Silverstripe project.
    
    ss_install_site: no    
    
Silverstripe environment.
    
    ss_env_type: dev
    
Silverstripe admin account name.
    
    ss_account_name: admin
    
Silverstripe admin account password.
    
    ss_account_pass: admin
    
Silverstripe path to sake. Relative to project root.
    
    ss_sake_path: /framework/sake


# beetbox

https://github.com/beetboxvm/beetbox

## Requirements

* [Vagrant](https://www.vagrantup.com/) >= 1.8
* [Virtualbox](https://www.virtualbox.org/)
* [Vagrant Hostsupdater](https://github.com/cogitatio/vagrant-hostsupdater)
* [Vagrant Auto-network](https://github.com/oscar-stack/vagrant-auto_network)

## Quickstart

  1. Open terminal (or [git bash](https://msysgit.github.io/) for windows users) and run the following commands --

  ```
  git clone https://github.com/beetboxvm/ansible-role-beetbox-silverstripe.git silverstripe && cd $_
  vagrant up
  ```

  2. Go to http://silverstripe.local/

  ```
  username: admin
  password: admin
  ```

## License

MIT
