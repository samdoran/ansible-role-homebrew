This role has moved to the collection [samdoran.macos](https://github.com/samdoran/ansible-collection-macos).

To switch to the collection, install the collection:

    ansible-galaxy collection install samdoran.macos

Then update tasks to use the fully qualified collection name:

```yaml
roles:
  - samdoran.macos.homebrew
```
