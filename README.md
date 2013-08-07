# Alpine Linux - Ansible Contrib Repository

This repository contains user-contributed real world examples for Ansible
playbooks, especially for Alpine Linux, as well as modules that are not a part
of Ansible's core distribution.

This is designed to be a resource to folks learning configuring Alpine Linux
with Ansible, as well as a way to share useful resources of all kinds.

If you have just found Ansible or Alpine Linux, you should start here:

 * [Alpine Linux](http://www.alpinelinux.org)
 * [Ansible project](https://github.com/ansible/ansible) -- see the examples directory

## Prerequisites

The [Documentation](http://wiki.alpinelinux.org/wiki/Ansible) helps
you to get started.

## Structure

At the moment the structure of the repository looks like this:

```bash
.
├── files ----------- Template files
├── handlers -------- Handlers for Alpine Linux services
├── maintenance ----- Complete playbooks
├── maintenance.yml - Regular tasks to perform on a running system
├── modules --------- Modules especially for Alpine Linux
├── README.md ------- This files
├── tasks ----------- A collection of tasks
├── setup.yml ------- Collected tasks for a fresh installed system
└── variables ------- Storage files for variables
```

## Warning
*Think first* before you implement stuff from this repository. Consider the 
playbooks in this repository as a show case. Somethings doesn't make sense, are
nasty hacks, or easier to do with another approach. 

## Licensing

Examples and modules should be licensed GPLv3 per the rest of Ansible, to
encourage modules to graduate from contrib to core.

All playbook content is assumed to be Creative Commons 3.0 Attribution licensed. 
Non-commerical or No-derivatives CC extensions are not acceptable, to encourage
easy use by all users, regardless of purpose.
