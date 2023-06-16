# Ansible gitea act runner

Ansible role to install and configure a [gitea act runner](https://gitea.com/gitea/act_runner).

## :warning: Warning :warning:

The runner and docker are setup as root, if you use it for a shared instance use a rootless setup!

## Requirements

None.

## Example playbook

````yaml
- hosts: all
  become: yes

  roles:
  - morbidick.act_runner

  vars:
    act_runner_instance: https://your.instance
    act_runner_token: abcde
````

## License

MIT
