```
# Set some environment variables to keep everything local to our project
export ANSIBLE_PROJECT_ROOT=$PWD
export ANSIBLE_HOME=$PWD/.cache/.ansible
export ANSIBLE_REMOTE_TMP=$PWD/.cache/.ansible/tmp

# Since our molecule playbooks are not adjacent to collection directory, we need to set the ANSIBLE_COLLECTIONS_PATH
export ANSIBLE_COLLECTIONS_PATH=$PWD/collections

# Molecular will use the XDG_CACHE_HOME to store its ephemeral data
export XDG_CACHE_HOME=$PWD/.cache


molecule test
```
