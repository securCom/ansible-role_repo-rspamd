[![Build Status](https://www.travis-ci.org/securCom/ansible-role_repo-nginx.svg?branch=master)](https://www.travis-ci.org/securCom/ansible-role_repo-nginx)
[![GitHub release](https://img.shields.io/github/release/securCom/ansible-role_repo-nginx.svg)](https://github.com/securCom/ansible-role_repo-nginx)


# Repo: RSPAMD

Manage RSPAMD official repositories.

# Requirements

For supported systems  see https://rspamd.com/downloads.html. If yhour system is not supported,
the role tasks will be skipped.

For supported system by this role, see the `vars/os-<system>` files.

Feel free to add any new linux distribution and version if missing.

# Role Variables

- `rspamd_repo_state`: define presence of the repository

# Dependencies

There no external dependencies.

# Example Playbook

To install role, add following line to **ansible-galaxy** requirements file
```
- src: https://github.com/securCom/ansible-role_repo-rspamd
  version: master
  name: securcom.repo_rspamd
```

```
- hosts: servers
  roles:
     - securcom.repo_rspamd
```

# License

BSD

# Author Information

- Peter Hudec (@hudecof)