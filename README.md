Homebrew
=========

Install Xcode command line tools, Homebrew command line tools, and Homebrew Cask GUI apps.

Requirements
------------

- Ansible installed

Role Variables
--------------
| Name              | Default Value       | Description          |
|-------------------|---------------------|----------------------|
| `homebrew_taps` | `[undefined]` | List of Homebrew taps to add |
| `homebrew_packages` | `[see defaults/main.yml]` | List of Homebrew packages to install |
| `homebrew_cask_apps` | `[see defaults/main.yml]` | List of Homebrew Cask apps to install |
| `homebrew_cask_appdir` | `~/Applications` | Directory where Cask applications are installed |
| `homebrew_caskroom` | `/opt/homebrew-cask/Caskroom` | Where Cask applications will be stored. |

Example Playbook
----------------


    - hosts: localhost
      roles:
         - role: sdoran.homebrew
           homebrew_cask_appdir: "/Applications"

License
-------

MIT
