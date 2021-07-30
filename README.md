# WIP Ansible Role: buildkite-agent

not usable yet

[![Main](https://github.com/pellegrino/ansible-buildkite-agent/workflows/main/badge.svg?event=push)](https://github.com/pellegrino/ansible-buildkite-agent/actions?query=workflow%3Amain)

Installs a buildkite-agent on a RedHat/CentOS/OracleOS Linux or Debian/Ubuntu Linux servers.

## Requirements

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

## Supports

This playbook is continuously tested using Molecule for the following distros:

- centos8
- debian10
- debian9
- fedora32
- ubuntu1804
- ubuntu2004

Doesn't support windows or mac hosts yet.

## Role Variables

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Required var:

- buildkite_agent_token: YOUR AGENT TOKEN.

You may use ansible-vault or another secret management solution such as hashicorp vault to encrypt your buildkite agent token and handle this information securely.

## Dependencies

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - role: pellegrino.buildkiteagent
           vars:
             buildkite_agent_token: __YOUR_TOKEN_HERE__

## License

BSD

## Author Information

Vitor Pellegrino <pellegrino@linux.com>
