# workspace

[![Source Code](https://img.shields.io/badge/github-source%20code-blue?logo=github&logoColor=white)](https://github.com/rolehippie/ngrok)
[![General Workflow](https://github.com/rolehippie/ngrok/actions/workflows/general.yml/badge.svg)](https://github.com/rolehippie/ngrok/actions/workflows/general.yml)
[![Readme Workflow](https://github.com/rolehippie/ngrok/actions/workflows/docs.yml/badge.svg)](https://github.com/rolehippie/ngrok/actions/workflows/docs.yml)
[![Galaxy Workflow](https://github.com/rolehippie/ngrok/actions/workflows/galaxy.yml/badge.svg)](https://github.com/rolehippie/ngrok/actions/workflows/galaxy.yml)
[![License: Apache-2.0](https://img.shields.io/github/license/rolehippie/ngrok)](https://github.com/rolehippie/ngrok/blob/master/LICENSE)
[![Ansible Role](https://img.shields.io/badge/role-rolehippie.ngrok-blue)](https://galaxy.ansible.com/rolehippie/ngrok)

Ansible role to install ngrok local tunnel proxy.

## Sponsor

Building and improving this Ansible role have been sponsored by my current and previous employers like **[Cloudpunks GmbH](https://cloudpunks.de)** and **[Proact Deutschland GmbH](https://www.proact.eu)**.

## Table of content

- [Requirements](#requirements)
- [Default Variables](#default-variables)
  - [ngrok_arch](#ngrok_arch)
  - [ngrok_keyring](#ngrok_keyring)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Requirements

- Minimum Ansible version: `2.10`

## Default Variables

### ngrok_arch

Architecture for ngrok repo

#### Default value

```YAML
ngrok_arch: "{{ 'arm64' if ansible_architecture == 'aarch64' else 'amd64' }}"
```

### ngrok_keyring

Path for the repository keyring

#### Default value

```YAML
ngrok_keyring: /usr/share/keyrings/ngrok-archive-keyring.gpg
```

## Discovered Tags

**_ngrok_**

## Dependencies

- None

## License

Apache-2.0

## Author

[Thomas Boerger](https://github.com/tboerger)
