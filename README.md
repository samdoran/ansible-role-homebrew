Homebrew
=========

Install Xcode command line tools, Homebrew command line tools, and Homebrew Cask GUI apps.

Requirements
------------

- Ansible installed

Role Variables
--------------
List taps to be installed

    homebrew_taps:
      - caskroom/cask

List packages to be installed:

    homebrew_packages:
      - fish
      - htop
      - coreutils
      - iperf
      - nmap
      - ssh-copy-id
      - tmux
      - watch
      - wget
      - git

List Homebrew Cask apps to be installed

    homebrew_cask_apps:
      - google-chrome

Where Cask apps are symlinked:

    homebrew_cask_appdir: "~/Applications"

Define the Caskroom:

    homebrew_caskroom: "/opt/homebrew-cask"


Example Playbook
----------------


    - hosts: localhost
      roles:
         - { role: sdoran.homebrew, homebrew_cask_appdir: "/Applications" }

License
-------

MIT
