# Arch Linux User Setup

Creates User

## Requirements

It should work on any archlinux distribution

## Role Variables

| Variable                     | Required | Default | Choices         | Comments                                       |
| ---------------------------- | -------- | ------- | --------------- | ---------------------------------------------- |
| archlinux_user\_\_name       | yes      |         |                 | name of the user to be created                 |
| archlinux_user\_\_groups     | no       | []      |                 | list of groups user should be added to         |
| archlinux_user\_\_privileged | no       | true    | true, false     | true to allow root privileges, false otherwise |
| archlinux_user\_\_state      | no       | present | present, absent | present to install, absent to remove           |

## Example Playbook

    - hosts: archlinux
      roles:
        - role: eliseuvideira.archlinux_user
          archlinux_user__name: archlinux

## License

MIT
