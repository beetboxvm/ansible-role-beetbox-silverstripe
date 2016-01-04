# Ansible Role: Beetbox Silverstripe

An Ansible role that creates and installs a Silverstripe project on beetbox.

## Requirements

This role is specifically developed as an extention to beetbox -- https://github.com/drupalmel/beetbox

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


## Dependencies

- Beetbox -- https://github.com/drupalmel/beetbox

## License

MIT