Ansible Role: celery
====================

[![Build Status](https://travis-ci.org/ScorpionResponse/ansible-celery.svg?branch=master)](https://travis-ci.org/ScorpionResponse/ansible-celery)

Ansible role to install Celery.

Requirements
------------

None.

Role Variables
--------------

### Optional
* `celery_log_dir`: The directory to store logs.  Default: /var/log/celery
* `celery_user_name`: The user account to run celery under. Default:
  celery
* `celery_group_name`: The group to run celery under. Default: celery

Dependencies
------------

* The ScorpionResponse.pip role will be used to install pip
* The ScorpionResponse.supervisord role will be use to install supervisord and
  run celery with that.

Example Playbook
----------------

Example usage:

    - hosts: all
      roles:
         - { role: ScorpionResponse.celery }

License
-------

BSD

Author Information
------------------

Github: https://github.com/ScorpionResponse
