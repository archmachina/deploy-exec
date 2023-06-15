# cicd-tools
Continuous Integration and Continuous Deployment Tools

[![linting](https://github.com/archmachina/cicd-tools/workflows/latest-linting/badge.svg)](https://github.com/archmachina/cicd-tools/actions?query=workflow%3Alatest-linting)
[![testing](https://github.com/archmachina/cicd-tools/workflows/latest-testing/badge.svg)](https://github.com/archmachina/cicd-tools/actions?query=workflow%3Alatest-testing)


## ansible-entrypoint
ansible-entrypoint provides a wrapper to call the ansible-playbook command. The wrapper performs the following functions:
* Creates a python venv for install of ansible and python packages
* Installs pip and python packages as per requirements.txt
* Installs ansible collections and roles as per requirements.yml

Example:
```bash
./cicd-tools/ansible-entrypoint ./main.yml -i ./inventory/dev/ -v
```

ansible-entrypoint will set ANSIBLE_HOME to the <PLAYBOOK_DIR>/.ansible, where any roles or collections will be installed.

## azd_env_promote

## env_vault

## next_environment

