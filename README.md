# Ansible Role: qBittorrent nox

[![Build Status](https://img.shields.io/travis/com/webplates/ansible-role-xtrabackup.svg?style=flat-square)](https://travis-ci.com/webplates/ansible-role-xtrabackup)
[![Ansible Galaxy](http://img.shields.io/badge/galaxy-webplates.xtrabackup-5fb7b9.svg?style=flat-square)](https://galaxy.ansible.com/webplates/xtrabackup)

Installs [qBittorrent](https://www.qbittorrent.org/) nox (no X) on Debian and Ubuntu (Raspbian too).


## Role Variables

| Variable | Default | Description |
| -------- | ------- | ----------- |
| `qbittorrent_nox_package_state` | `present` | Package state (`present` or `latest` to upgrade) |
| `qbittorrent_nox_user` | `qbtuser` | Service user name |
| `qbittorrent_nox_user_groups` | `[]` | Additional groups to add the service user to |
| `qbittorrent_nox_webui_port` | `8080` | WebUI port number |


## Example Playbook

```yaml
    - hosts: servers
      roles:
         - { role: sagikazarmark.qbittorrent_nox }
```


## License

The MIT License (MIT). Please see [License File](LICENSE) for more information.
