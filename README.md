| CI Status|
|------|
|![molecule test](https://github.com/NiftyMist/niftymist.baseline/actions/workflows/molecule.yml/badge.svg)|

niftymist.baseline
=========

A baseline configuration.  Sets up users and ssh keys and installs packages that I like to have installed on all my systems.

Requirements
------------

None

Role Variables
--------------

| Variable | Required? | Default | Notes |
|------|------|------|------|
| baseline_packages | yes | `vim` and `zsh` | list of packages to install |
| baseline_ansible_user | no | `ansible` | user to be created for ansible automation |
| baseline_ansible_password | yes | N/A | ansible user password encrypted |
| baseline_standard_user | yes | N/A | user to be created for non automated use |
| baseline_standard_password | yes | N/A | standard user password encrypted |
| baseline_ansible_user_pub_key_url | no | `""` | url to ansible user public key to be installed |
| baseline_standard_user_pub_key_url | no | `""` | url to standard user public key to be installed |

Dependencies
------------

N/A

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      become: yes
      roles:
         - nfitymist.baseline

License
-------

BSD

Author Information
------------------

Dylan Mitchell
mdmitch92@gmail.com
# niftymist.baseline
