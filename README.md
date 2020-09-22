# Ansible Role: ansible-apps_logstash_exporter


## Description

[![Build Status](https://travis-ci.com/lotusnoir/ansible-apps_logstash_exporter.svg?branch=master)](https://travis-ci.com/lotusnoir/ansible-apps_logstash_exporter)[![License](https://img.shields.io/badge/license-MIT%20License-brightgreen.svg)](https://opensource.org/licenses/MIT)[![Ansible Role](https://img.shields.io/badge/ansible%20role-apps__logstash_exporter-blue)](https://galaxy.ansible.com/lotusnoir/ansible-apps_logstash_exporter/)[![GitHub tag](https://img.shields.io/badge/version-latest-blue)](https://github.com/lotusnoir/ansible-apps_logstash_exporter/tags)

Deploy [logstash_exporter](https://gitlab.com/alxrem/prometheus-logstash-exporter) using ansible.


## Role variables

| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
| `logstash_exporter_version` | 0.6.2 | logstash_exporter version |
| `logstash_exporter_port` | :9114 | Prometheus endpoint |
| `logstash_exporter_loglevel` | info | log level  |

## Examples

	---
	- hosts: apps_logstash_exporter
	  become: yes
	  become_method: sudo
	  gather_facts: yes
	  roles:
	    - role: ansible-apps_logstash_exporter
	  environment: 
	    http_proxy: "{{ http_proxy }}"
	    https_proxy: "{{ https_proxy }}"
	    no_proxy: "{{ no_proxy }}


## License

This project is licensed under MIT License. See [LICENSE](/LICENSE) for more details.
