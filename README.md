# Ansible Role: qBittorrent nox

[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/sagikazarmark/ansible-role-qbittorrent-nox/CI?style=flat-square)](https://github.com/sagikazarmark/ansible-role-qbittorrent-nox/actions?query=workflow%3ACI)
[![Ansible Galaxy](http://img.shields.io/badge/galaxy-sagikazarmark.qbittorrent_nox-5fb7b9.svg?style=flat-square)](https://galaxy.ansible.com/sagikazarmark/qbittorrent_nox)

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
