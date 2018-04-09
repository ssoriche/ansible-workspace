# ansible-workspace

This project is being created to mitigate frustration when starting work in a
new environment. The idea is these playbooks and roles are used to maintain
various systems ranging from local workstations where full control is allowed,
to remote servers on customer premises with only ssh access.

## Roles

### git_local_checkout

This role connects to a remote git repository and checks it out into a local
work directory. Projects like [Anyenv](https://github.com/riywo/anyenv) require
a `git clone` in order to install. Systems without Internet access, or limited
access, will not be able to clone the repository. Using `git_local_checkout`,
Ansible can be configured to copy the local checkout to the remote server.
