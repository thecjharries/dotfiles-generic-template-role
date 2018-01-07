# `dotfiles-role-generic-template`

[![Build Status](https://travis-ci.org/thecjharries/dotfiles-role-generic-template.svg?branch=master)](https://travis-ci.org/thecjharries/dotfiles-role-generic-template)

## Requirements

Fedora 27 is recommended.

## Role Variables

Defaults are below.

```yml
---
owning_user: "{{ ansible_user }}"
owning_group: "{{ ansible_user }}"
template_root: "/home/{{ ansible_user }}"
```

Finally, these variables must be set:

```yml
template_path
```

## Dependencies

None

## Example Playbook

```yml
---
- hosts: all

  roles:
    - role: dotfiles_generic_template
      template_path: "some/file"
```

## License

ISC
