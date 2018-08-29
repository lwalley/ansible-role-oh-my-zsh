# Ansible Role: Oh My Zsh

Installs [Oh my Zsh][ohmyzsh] on Mac OS.

## Requirements

[Zsh][zsh] must be installed on the system prior to running this role. Zsh is
pre-installed on Mac OS X, if you want to update to a later version consider
using [Homebrew][brew] (suggested role: `geerlingguy.homebrew`).

## Role Variables

None.

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
