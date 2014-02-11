Wordpress
=========

Downloads and install wordpress and sets it up to run with uwsgi.
This setup makes clever use of a read-only `bind mount` of the wordpress
source in the uwsgi dir.


Requirements
------------

The role is created for Debian-like OS's. Depends on the uWSGI role, and also installs nginx as a frontend.


Role Variables
--------------

The role uses the following variables, that you can also override:

* `wordpress_hostname` - the hostname of the site
* `wordpress_user` - system user id to run the wordpress site as
* `wordpress_db_name` - database name
* `wordpress_db_user` - database user
* `wordpress_db_password` - database password
* `wordpress_db_host` - database host, defaults to localhost
* `wordpress_version` - updated to match the latest version


Usage
-----

    ansible-galaxy install gdamjan.wordpress

Also check the [Ansible Galaxy](https://galaxy.ansibleworks.com/intro) about page.


License
-------

BSD

Author and other Information
----------------------------

Damjan Georgievski

[GitHub project page](https://github.com/gdamjan/ansible-wordpress)

