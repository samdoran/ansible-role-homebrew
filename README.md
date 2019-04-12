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

Example Playbook
----------------


    - hosts: localhost
      roles:
         - role: samdoran.homebrew
           homebrew_cask_appdir: "/Applications"

License
-------

Apache 2.0
