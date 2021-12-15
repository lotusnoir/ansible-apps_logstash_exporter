# ansible-apps_logstash_exporter

## Description

[![Galaxy Role](https://img.shields.io/badge/galaxy-apps_logstash_exporter-purple?style=flat)](https://galaxy.ansible.com/lotusnoir/apps_logstash_exporter)
[![Version](https://img.shields.io/github/release/lotusnoir/ansible-apps_logstash_exporter.svg)](https://github.com/lotusnoir/ansible-apps_logstash_exporter/releases/latest)
![GitHub repo size](https://img.shields.io/github/repo-size/lotusnoir/ansible-apps_logstash_exporter?color=orange&style=flat)
[![downloads](https://img.shields.io/ansible/role/d/52259)](https://galaxy.ansible.com/lotusnoir/apps_logstash_exporter)
![Ansible Quality Score](https://img.shields.io/ansible/quality/52259)
[![License](https://img.shields.io/badge/license-Apache--2.0-brightgreen?style=flat)](https://opensource.org/licenses/Apache-2.0)

Deploy [logstash_exporter](https://gitlab.com/alxrem/prometheus-logstash-exporter) using ansible.

## Requirements

none

## Role variables

See [variables](/defaults/main.yml) for more details.

## Examples

        ---
        - hosts: apps_logstash_exporter
          become: true
          become_method: sudo
          gather_facts: true
          roles:
            - role: ansible-apps_logstash_exporter

## Grafana Dashboard

You can find a grafana dashboard [here](https://grafana.com/grafana/dashboards/13572)

## License

This project is licensed under Apache License. See [LICENSE](/LICENSE) for more details.

