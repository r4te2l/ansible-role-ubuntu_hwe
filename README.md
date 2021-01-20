Ubuntu HWE
=========

Manages Ubuntu HWE Packages

Requirements
------------

N/A

Role Variables
--------------

| Variable                 | Purpose                                        | Default                                                    |
| ------------------------ | ---------------------------------------------- | ---------------------------------------------------------- |
| ubuntu_hwe_packages      | List of Packages to manage                     | [ "linux-generic-hwe-{{ ansible_distribution_version }}" ] |
| ubuntu_hwe_package_state | State of HWE Packages                          | 'latest'                                                   |
| ubuntu_hwe_apt_update    | Run Apt Update prior to installing HWE Package | true                                                       |

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in
regards to parameters that may need to be set for other roles, or variables that
are used from other roles.

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
     - { role: ubuntu_hwe }

```

License
-------

BSD
