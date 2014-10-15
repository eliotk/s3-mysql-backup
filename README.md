s3-mysql-backup
===============

Ansible role for setting up a daily automatic backup of all mysql databases to s3.

#### Usage

Add the role to the playbook like this, setting the necessary vars:

```
- name: My playbook
  hosts: my_server
  roles:
  - role: mysql-s3-backup
    s3_mysql_backup_mysql_root_password: ...
    s3_mysql_backup_bucket_name: ...
    s3_mysql_backup_s3_access_key: ...
    s3_mysql_backup_s3_access_token: ...
    s3_mysql_backup_additional_cron_cmd: ...
```

### Credits

Utilizes Github user oodavid's gist and script:

https://gist.github.com/oodavid/2206527