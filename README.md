# Prerequisites

- Poetry[^1]
- mise (optional)[^2]

# Setup

``` bash
poetry install
```

# How to use

## Add role

``` bash
cd roles
poetry run ansible-galaxy role init [role_name]

# optional (for testing)
cd [role_name]
poetry run molecule init scenario
```

## Run playbook

``` bash
# poetry run ansible-playbook -i [inventory_name] site.yml
poetry run ansible-playbook -i development site.yml
```

[^1]: <https://python-poetry.org/>

[^2]: <https://mise.jdx.dev/>
