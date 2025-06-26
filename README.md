export CA_PASSPHRASE='hkgfkhghgfjkasdhgfjag'

# write these values as vars to extra_vars/ca.yml
ansible-playbook playbook-generate-ca.yml

ansible-playbook playbook-issue-certificate.yml -e @extra_vars/ca.yml