[![Build Status](https://api.travis-ci.org/votum/ansible-role-githook-for-jira.svg?branch=master)](https://travis-ci.org/votum/ansible-role-githook-for-jira)

# githook for jira

installs a local githook for jira

username in git config must be in shape of surename.lastname
commit message must be in shape of:

```
some text BIO-25 some text

the long message 
will be send to Jira as comment.
```

subject of commit message is parsed for Ticket ID.

## installation

set parameters in default/main.yml to your needs. and run:

```
ansible-galaxy install votum.githook-for-jira --roles-path=./etc/ansible/roles
```

