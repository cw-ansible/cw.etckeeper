<!--

---
lang: american
---
-->

[![Build Status](https://travis-ci.org/cw-ansible/cw.etckeeper.svg?branch=master)](https://travis-ci.org/cw-ansible/cw.etckeeper)
[![Tweet this](http://img.shields.io/badge/Tweet-it00aced.svg)](https://twitter.com/intent/tweet?tw_p=tweetbutton&via=renard_0&url=https%3A%2F%2Fgithub.com%2Fcw-ansible%2Fcw.etckeeper&text=Install%20and%20configure%20%23etckeeper%20using%20%23Ansible.)
[![Follow me on twitter](http://img.shields.io/badge/Twitter-Follow-00aced.svg)](https://twitter.com/intent/follow?region=follow_link&screen_name=renard_0&tw_p=followbutton)


# etckeeper

Install and configure [etckeeper](https://github.com/joeyh/etckeeper) into a
server.

## Usage

Include the `etckeeper` module to your playbook.

## Description

This will install both `etckeeper_vcs_pkg` and `etckeeper` packages, then
configure `etckeeper` to use `etckeeper_vcs` as VCS.

Finally the `etckeeper` initialization is done, the user and email
configured, then the first commit is done.

## Configuration

- `etckeeper_vcs`: name of VCS to use (default: `git`);
- `etckeeper_vcs_pkg`: package to install for `etckeeper_vcs` to work
  (default: `git`);
- `etckeeper_vcs_git_name`: name of `git` commiter (default `etckeeper`);
- `etckeeper_vcs_git_email`: email of `git` commiter (default
  `etckeeper@example.com`);


## Copyright

Author: Sébastien Gross `<seb•ɑƬ•chezwam•ɖɵʈ•org>` [@renard_0](https://twitter.com/renard_0)

License: WTFPL, grab your copy here: http://www.wtfpl.net
