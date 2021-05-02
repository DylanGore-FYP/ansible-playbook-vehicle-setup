# ansible-playbook-vehicle-setup

<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=for-the-badge)](#contributors)
<!-- ALL-CONTRIBUTORS-BADGE:END -->
<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/DylanGore-FYP/ansible-playbook-vehicle-setup/lint-playbook?label=Lint&logo=github&style=for-the-badge)](https://github.com/DylanGore-FYP/ansible-playbook-vehicle-setup/actions/workflows/lint.yml)

An Ansible Playbook that performs initial setup for the Raspberry Pi that will run the vehicle code.

## Requirements

- Python 3
- Ansible
- Git

## Configuration

1. Copy `vars/vars.yml` to `vars.yml` and edit the variables accordingly.
2. Add a `config.toml` file to the templates directory based on the example from the [DylanGore-FYP/Car](https://github.com/DylanGore-FYP/Car/blob/main/config.sample.toml).

## Running the Playbook

Get the required roles from Ansible Galaxy:

```bash
ansible-galaxy install -r requirements.yml -p roles --force
```

Run the playbook using SSH Key authentication:

```bash
ansible-playbook -i inventory playbook.yml
```

Run the playbook using password authentication:

```bash
ansible-playbook -i inventory playbook.yml --ask-pass
```

## Commit Message Convention

This project uses [Gitmoji](https://gitmoji.dev/) for commit organisation. For more details see the [Gitmoji Repository](https://github.com/carloscuesta/gitmoji).

## Contributors

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://github.com/DylanGore"><img src="https://avatars.githubusercontent.com/u/2760449?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Dylan Gore</b></sub></a><br /><a href="https://github.com/DylanGore-FYP/ansible-playbook-vehicle-setup/commits?author=DylanGore" title="Code">💻</a> <a href="https://github.com/DylanGore-FYP/ansible-playbook-vehicle-setup/commits?author=DylanGore" title="Documentation">📖</a> <a href="#ideas-DylanGore" title="Ideas, Planning, & Feedback">🤔</a></td>
    <td align="center"><a href="https://github.com/mohittaneja7"><img src="https://avatars.githubusercontent.com/u/4126813?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Mohit Taneja</b></sub></a><br /><a href="#ideas-mohittaneja7" title="Ideas, Planning, & Feedback">🤔</a></td>
  </tr>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification.
