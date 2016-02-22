[![Build Status](https://travis-ci.org/nlap/ansible-role-graph-tool.svg?branch=master)](https://travis-ci.org/nlap/ansible-role-graph-tool)

graph-tool Ansible Role
=========

An (unofficial) ansible role to install [graph-tool](http://graph-tool.skewed.de) and all of its prerequisites on Ubuntu/Debian.

Requirements
------------

Currently works with the recent Ubuntu/Debian distributions that have a supported graph-tool package.

See http://graph-tool.skewed.de/download for a list of supported releases. Pull requests are welcome!

Ansible 1.6 or higher required

Role Variables
--------------

By default this role installs graph-tool for Python 3 only.

You install graph-tool on different Python versions with these variables:

	graph_tool_python2: true
	graph_tool_python3: true
	
Set both to false to install only the dependencies.	

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: nlap.graph_tool

Dependencies
------------
None

License
-------

GPLv3