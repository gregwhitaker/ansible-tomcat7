ansible-tomcat7
=========

Ansible role that installs the Apache Tomcat7 application server.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

* `tomcat_user` - System user for Tomcat
* `tomcat_xmx` - Maximum heap memory size for Tomcat
* `tomcat_extra_opts` - Extra command line parameters to supply to the Tomcat JVM during startup

Dependencies
------------

This role requires the `java8` role which can be installed by running the following command:

	$ ansible-galaxy install -r requirements.yml

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: tomcat7, tomcat_xmx: 1024 }

License
-------

Apache
