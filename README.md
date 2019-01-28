[![Build Status](https://travis-ci.com/calvinbui/ansible-duplicacy.svg?branch=master)](https://travis-ci.com/calvinbui/ansible-duplicacy)

# Ansible Duplicacy

Installs Duplicacy and uses Dropbox as backup location.

Add things into the pre-backup.sh script if things need to be done before the backup begins.

##  Requirements

N/A

## Role Variables

`duplicacy_version`: Version to install

`duplicacy_url`: Where to download from

`duplicacy_dropbox_folder`: Dropbox to place backups in

`duplicacy_dropbox_token`: Dropbox backup token

`duplicacy_backup_folder`: Folder to backup


## Dependencies

N/A

## Example Playbook

```yaml
- hosts: servers
  become: true
  roles:
    - role: calvinbui.ansible_duplicacy
```

## License

GPLv3

## Author Information

http://calvin.me
