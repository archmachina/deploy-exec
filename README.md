# deploy-exec
Deployment utility scripts

[![linting](https://github.com/archmachina/deploy-exec/workflows/latest-linting/badge.svg)](https://github.com/archmachina/deploy-exec/actions?query=workflow%3Alatest-linting)
[![testing](https://github.com/archmachina/deploy-exec/workflows/latest-testing/badge.svg)](https://github.com/archmachina/deploy-exec/actions?query=workflow%3Alatest-testing)


## ansible-entrypoint
ansible-entrypoint provides a wrapper to call the ansible-playbook command. The wrapper performs the following functions:
* Creates a python venv for install of ansible and python packages
* Installs pip and python packages as per requirements.txt
* Installs ansible collections and roles as per requirements.yml

Example:
```
./deploy-exec/ansible-entrypoint ./main.yml -i ./inventory/dev/ -v
```

ansible-entrypoint will set the HOME directory to the playbook directory and any roles, collections, python modules or caches will be stored there.

## azd_env_promote

## env_vault

## next_environment

