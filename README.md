# [here the name of your Ansible Playbook / Role ]

## Description

This repository contains an **[name here]** that automates [describe the purpose of the playbook or role]. 

## Prerequisites and dependecies

Before running the playbook, make sure you have the following requirements available:

- **Ansible**: Version 2.x or later.
- Access to the target systems / services with appropriate permissions.
- (Optional) Additional dependencies specified in the `requirements.yml` or `requirements.txt` files.

## Repository Structure


```
.
├── README.md
├── defaults
│   └── main.yml
├── files
├── handlers
│   └── main.yml
├── meta
│   └── main.yml
├── roles
├── tasks
│   └── main.yml
├── templates
├── tests
│   ├── inventory
│   └── test.yml
└── vars
    └── main.yml
```

## Role Vars


Variable Name | Description | Example | Default value |
|:-------------------|:-------------------|:-------------------| :-------------------|
__base_url__(string) | The API endpoint base path | https://endpoint2.com | https://endpoint1.com |


## Extra Vars

(Optional) You can use extra-vars as plain text or by survey method. If your playbook do not have extra-vars the table must be empty 

Variables | Comments | Example | Default |
|:-------------------|:-------------------|:-------------------| :-------------------|
__hostname__(String) | Is the host involved | linuxAXUP3 |


## Usage of the rol

If you want to run the playbook use the following code:

Example:
 
```
- name: Description of the role
  hosts: localhost
  connection: local
  ....

  tasks:
    - name: Include rol X
      include_role:
        name: here the name of your role
      vars:
        base_url: "{{ base_url }}
```

## Author Information

Ansible developer name - Ansible developer email