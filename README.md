# Ansible Role: aap-uninstall 

Simple role to uninstall Ansible Automation Platform.

## Requirements
No requirements as this role will remove AAP installed on any systems this role is run against.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

Below is a list of all basic variables used throughout the role.

| Variable | Description | Required | Defaults |
|:--------:|:-----------:|:--------:|:--------:|
| **aap_uninstall** | Do you want to uninstall aap | yes | yes |

## Dependencies

None.

## Example Playbook

    - hosts: aap
      become: yes
      vars_files:
        - vars/main.yml
      roles:
        - ansible-role-aap-uninstall

*Inside `vars/main.yml`*:
    aap_uninstall: true


## License

MIT / BSD

## Author Information

This role was created in 2023 by [Ken Hitchcock](https://github.com/kenhitchcock).
