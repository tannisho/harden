---
created roles for execution ordering (ie: run pkgs role before auditd role to
install auditd role package dependancies)

prerequisites:
update 'inventory' and 'roles_path' to repo path (ie: ~/harden/inventory.yml)
update 'vars_files' to repo path (ie: ~/harden/var/external_vars.yml)

ansible-playbook --user username --ask-pass --become-user root --ask-become-pass foo.yml
