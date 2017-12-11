ansible-hel-django
==================

An Ansible role to build/deploy Django applications as built within the Open
Software Development within City of Helsinki.

Role Variables
--------------

* django_user: user the applications will run as
* django_name: This is the directory the source code if checked out to, also the prefix for all cookies
* django_pillow: Whether to install pillow Ubuntu dependencies
* django_lxml: Whether to install packages needed for lxml Python module
* django_git_url: Where to check out the source code from
* django_git_version: Which treelike to check out from git
* django_git_force_pull: force pull, only meaningful if there is an existing checkout at destination
* django_full_reinit: #This only runs manage.py rebuild_index
* django_config_fragments: list any config fragment files for Hel-style local_settings
* django_service_pypis: list any additional pypis needed
* django_setup_commands: list any admin commands to be run for setup
* django_virtualhosts: list of virtualhosts the application will serve
* django_url_prefix: Prefix expected/stripped for all incoming requests

License
-------

BSD

Author Information
------------------

Created by Ville Koivunen <ville.koivunen@hel.fi>. Angry feedback welcome.
