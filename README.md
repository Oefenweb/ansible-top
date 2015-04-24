## top

[![Build Status](https://travis-ci.org/Oefenweb/ansible-top.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-top) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-top-blue.svg)](https://galaxy.ansible.com/list#/roles/1725)

Set up top in Debian-like systems.

#### Requirements

None

#### Variables

* `top_toprc_destinations`: [default: `{skell: dest: /etc/skel, current: dest: "{{ ansible_env.HOME }}"}`]: Destinations to copy the toprc file to
* `top_replace_toprc`: [default: `true`]: Whether or not to overwrite existing toprc files

## Dependencies

None

#### Example

```yaml
---
- hosts: all
  roles:
  - top
```

#### License

MIT

#### Author Information

Mischa ter Smitten

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/Oefenweb/ansible-top/issues)!
