# Ansible Role: Zammad

This Ansible role automates the installation and configuration of Zammad, a web-based ticketing system and customer support platform.

## Requirements

- Ansible installed on the control node.
- Target system must meet the minimum system requirements for Zammad.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

- `zammad_package_state`: Sets the state of the Zammad package. Default is `present`.
- `zammad_apt_priority`: Set zammad repo priority for apt. Default is `100` (bellow apt default priority which is 500).
- `zammad_nginx_disable_default_web_server`: Disable the default nginx configuration shipped by the zammad package. Default is `true`.
- `zammad_add_redis`: Add redis or not to configuration. Default is `false`.

## Dependencies

None.

## Example Playbook

```yaml
- hosts: servers
  roles:
    - role: chadek.zammad
```

## License

This role is licensed under the MIT License.

## Author Information

This role was created by [Your Name Her.

## Feedback and Contributions

Please feel free to open an issue or submit a pull request on [GitHub](https://github.com/chadek/ansible-role-zammad) if you have any feedback or would like to contribute.
