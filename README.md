# [Install emacs24 with Ansible][https://github.com/thydel/ar-emacs24]

- Install emacs24-nox if emacs24 is not already installed
- Use backport if needed

  - Currently wheezy is the only known release to require use of backport
  
## Usage

Install via [Galaxy](https://galaxy.ansibleworks.com/):

```
ansible-galaxy install thydel.emacs24
```

## Dependencies

Need role [jnv.debian-backports](https://github.com/jnv/ansible-role-debian-backports)

## Example Playbook

```yaml
- hosts: all
   roles:
    - jnv.debian-backports
	- thydel.emacs24
```
