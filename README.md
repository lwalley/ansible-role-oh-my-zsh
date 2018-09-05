# Ansible Role: Oh My Zsh

Installs [Oh my Zsh][ohmyzsh] on Mac OS.

## Requirements

[Zsh][zsh] must be installed on the system prior to running this role. Zsh is
pre-installed on Mac OS X, if you want to update to a later version consider
using [Homebrew][brew] (suggested role: `geerlingguy.homebrew`).

## Role Variables

Available variables with example values are listed below, for default values see
[`defaults/main.yml`](defaults/main.yml)):

    oh_my_zsh_custom_themes:
      - repo: https://github.com/bhilburn/powerlevel9k.git
        name: powerlevel9k
    oh_my_zsh_custom_plugins:
      - repo: https://github.com/zsh-users/zsh-syntax-highlighting.git
        name: zsh-syntax-highlighting
    oh_my_zsh_active_theme: powerlevel9k/powerlevel9k
    oh_my_zsh_active_plugins:
      - git
      - zsh-syntax-highlighting

## Dependencies

None.

## Example Playbook

    - hosts: localhost
      roles:
         - { role: lwalley.oh-my-zsh }

## License

MIT

[brew]: https://brew.sh
[ohmyzsh]: https://github.com/robbyrussell/oh-my-zsh
[zsh]: http://www.zsh.org
