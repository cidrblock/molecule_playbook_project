```
ansible-creator init --project ansible-project --scm-org myorg --scm-project myproject --init-path molecule_playbook_project
cd molecule_playbook_project
export ANSIBLE_PROJECT_ROOT=$PWD
export ANSIBLE_HOME=$PWD/.cache/.ansible
export ANSIBLE_REMOTE_TMP=$PWD/.cache/.ansible/tmp
export ANSIBLE_COLLECTIONS_PATH=$PWD/collections
export XDG_CACHE_HOME=$PWD/.cache

molecule init scenario
```
