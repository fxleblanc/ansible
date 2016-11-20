# Ansible scripts

## Usage

### Install roles
```
ansible-galaxy -r requirements.yml
```
### Launch a playbook in production
```
ansible-playbook -i inventory/production -K [playbook-path]
```

## Development

### Launch the Vagrant vm
```
vagrant up
```
### Launch a playbook for development
```
ansible-playbook -i inventory/development [playbook-path]
```
Note: You don't need the -K option since the vagrant user doesn't need a password to become sudo
