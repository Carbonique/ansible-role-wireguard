- [About](#about)
- [Variables](#variables)

# About

Wireguard install for the lazy 

This role installs a pre-existing Wireguard config(default `etc/wireguard`) that has already been compressed into a `.tgz` file and encrypted using `ansible-vault`

The config `.tgz` has to be named `wireguard-encrypted.tgz`

# Variables

For defaults see `defaults/main.yml`.

| Variable                  | Description                       | Default | Optional/Required |
|---------------------------|-----------------------------------|---------|-------------------|
| tgz_path              | Path of the tgz file on the Ansible controller      | null    | Required          |
