# Odoo 16

## User Default Login Odoo:
- user: `user@example.com`
- password: `bitnami`

## Dependencies (optional)
- `apt install build-essential`
- `apt install wheels`
- `wget https://github.com/wkhtmltopdf/packaging/releases/download/0.12.6.1-2/wkhtmltox_0.12.6.1-2.bullseye_arm64.deb`
- `apt install ./wkhtmltox_0.12.6.1-2.bullseye_arm64.deb`
- `apt install libsasl2-dev python-dev libldap2-dev libssl-dev`

## Setup Postgres
`docker exec -it <container_code> psql -U postgres`

## Reference:
https://linuxhint.com/install-odoo-15-ubuntu-22-04/
