# Ansible Role: Dotfiles

[![Build status][ci-badge]][ci-url]

Simple yet elegant ansible role to install a set of dotfiles from a git repository.

## Requirements

Requires `git` to be installed on the managed machine.

## Parameters

| Name                            | Description                                                                                   | Default                                     | Required |
| ------------------------------- | --------------------------------------------------------------------------------------------- | ------------------------------------------- | -------- |
| dotfiles_repo                   | Dotfiles git repository                                                                       | https://github.com/vandycknick/dotfiles.git | no       |
| dotfiles_repo_version           | Tag or branch name to checkout                                                                | main                                        | no       |
| dotfiles_repo_accept_hostkey    | If yes, ensure that "-o StrictHostKeyChecking=no" is present as an ssh option.                | false                                       | no       |
| dotfiles_repo_local_destination | The path of were the dotfiles repository should be checked out                                | ~/Projects/dotfiles                         | no       |
| dotfiles_home                   | The path where dotfiles will be synced to, this most likely will be the users home directory. | ~                                           | no       |

## Dependencies

None

## Examples

```yaml
- hosts: localhost
  roles:
    - role: vandycknick.dotfiles
```

[ci-url]: https://github.com/vandycknick/ansible-role-dotfiles
[ci-badge]: https://github.com/vandycknick/ansible-role-dotfiles/workflows/CI/badge.svg
