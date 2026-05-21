# Ansible role week4_databaseserver

Deze role installeert MySQL op een Ubuntu databaseserver.

## Taken

- apt cache bijwerken
- mysql-server installeren
- python3-pymysql installeren
- mysql starten
- mysql enablen
- database week4db aanmaken
- gebruiker dbuser aanmaken met wachtwoord dbpassword

## Gebruik

```yaml
---
- name: Configureer databaseserver
  hosts: databaseservers
  become: true

  roles:
    - week4_databaseserver
