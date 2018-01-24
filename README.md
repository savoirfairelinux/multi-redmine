Ansible Multi Redmine Role
==========================

For Debian-based operating systems. Installs and configure Redmine from Git repo,
compatible with rbenv environments.


Requirements
------------

* Ansible 2.3+
* PostgreSQL 9.5+
* One of these target systems:
    * Debian Jessie
    * Ubuntu 16.04
* Ansible roles:
    * [puma-rbenv-nginx][ansible-puma-rbenv-nginx]
    * [gitpush-deploy][ansible-gitpush-deploy]
    * [postgresql][ansible-postgres-install]


Usage example
-------------

See [default variables](defaults/main.yml) for more variables.

```yaml
- role: redmine
  redmine_rails_environment: production
  redmine_database_password: SOMEPASSWORD
```


Conclusion
----------

We absolutely appreciate patches, feel free to contribute directly on the GitHub project.

Repositories / Development website / Bug Tracker:
- https://github.com/savoirfairelinux/ansible-multi-redmine.git

Do not hesitate to join us and post comments, suggestions, questions and general feedback directly on the issues tracker.

**Website :** https://www.savoirfairelinux.com/


[ansible-gitpush-deploy]: https://github.com/savoirfairelinux/ansible-gitpush-deploy
[ansible-postgres-install]: https://github.com/ANXS/postgresql
[ansible-puma-rbenv-nginx]: https://github.com/savoirfairelinux/ansible-puma-rbenv-nginx
