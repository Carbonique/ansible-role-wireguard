- [About](#about)
- [Installation](#installation)
- [Defaults](#defaults)

# About

Wireguard install for the lazy 

This role installs a pre-existing Wireguard config(default `etc/wireguard`) that has already been compressed into a `.tgz` file and encrypted using `ansible-vault`

The config `.tgz` has to be named `wireguard-encrypted.tgz`

# Installation

Add the following to `requirements.yml`:

```
- src: https://github.com/carbonique/ansible-role-wireguard.git
  scm: git
  name: wireguard
  version: #Leave empty for latest. To download a specific version: use the tag as listed in repo
```

For system wide installation:
`ansible-galaxy install -r requirements.yml`

For installation to the current directory:
`ansible-galaxy install --roles-path . -r requirements.yml`

# Defaults

Defaults have been prefilled. Variables have to be added by user

For defaults see: `defaults/main.yml`

