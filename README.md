[![Build Status](https://travis-ci.org/bihealth/ansible-role-jannovar-server.svg?branch=master)](https://travis-ci.org/bihealth/ansible-role-jannovar-server)

# Jannovar Server

Setup of Jannovar REST server.

## Requirements

None.

## Role Variables

See `defaults/main.yml` for all role variables and their documentation.

## Dependencies

- `bihealth.nginx`

## Example Playbook

```yaml
- hosts: servers
  vars:
    # bihealth.ssl_certs --------------------------------------------------------------------------
    ssl_certs_certs:
      - name: jannovar.example.com
  roles:
    - role: bihealth.jannovar_server
```

## License

MIT

## Author Information

- Manuel Holtgrewe

Created with love at [Core Unit Bioinformatics (CUBI), Berlin Institute of Health (BIH)](https://www.cubi.bihealth.org).
