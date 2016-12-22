## top

[![Build Status](https://travis-ci.org/Oefenweb/ansible-top.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-top) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-top-blue.svg)](https://galaxy.ansible.com/tersmitten/top)

Set up top in Debian-like systems.

#### Requirements

None

#### Variables

* `top_toprc_destinations`: [default: `{skell: dest: /etc/skel, current: dest: "{{ ansible_env.HOME }}"}`]: Destinations to copy the toprc file to
* `top_toprc_destinations.key`: The identifier of the file (e.g. `skel`)
* `top_toprc_destinations.key.dest`: The remote path of the file to copy (e.g. `/etc/skel`)
* `top_toprc_destinations.key.owner`: The name of the user that should own the file (optional, default `root`)
* `top_toprc_destinations.key.group`: The name of the group that should own the file (optional, default `owner`, then `root`)
* `top_toprc_destinations.key.mode`: The mode of the file, such as 0644 (optional, default `0644`)

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
