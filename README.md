# RHEL7 CIS Benchmark role
#### Security and operationaly harden RHEL and Fedora19+ via CIS benchmark Guidance

**Warning: This is very much a work in progress - Do not use this in a production capacity**


cd tests && ansible-playbook -i localhost, --e \"cis_level_1_exclusions=['3.2.8','5.3.4']\" playbook.yml --check

```bash
$ ansible-playbook -i localhost, --skip=1.1.18,1.1.19,1.2.2,1.3.1,1.3.2,1.5.4,1.7.1.5,1.7.1.6,2.1.11,2.1.6,2.1.7,2.1.8,2.1.9,2.1.10,2.2.1.1,2.2.2,2.2.3,2.2.4,2.2.5,2.2.6,2.2.7,2.2.8,2.2.9,2.2.10,2.2.11,2.2.12,2.2.13,2.2.14,2.2.15,2.2.16,2.3.1,2.3.2,2.3.3,2.3.4,2.3.5 --e \"cis_level_1_exclusions=['3.2.8','5.3.4']\" playbook.yml --check
```

todo switch from yum to dnf
switch from service status whatever to sytemD statuses
