Homebrew
=========

Install Xcode command line tools, Homebrew, Homebrew command line tools, and Homebrew Cask GUI apps.

Requirements
------------

- Ansible installed

Role Variables
--------------
| Name              | Default Value       | Description          |
|-------------------|---------------------|----------------------|
| `homebrew_taps` | `['homebrew/cask-drivers']` | List of Homebrew taps to add |
| `homebrew_packages` | `[]` | List of Homebrew packages to install |
| `homebrew_cask_apps` | `[]` | List of Homebrew Cask apps to install |

Example Playbook
----------------


    - hosts: localhost
      roles:
         - samdoran.homebrew


License
-------

Apache 2.0
