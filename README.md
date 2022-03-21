# Selfhosted server with ansible

## Usage

Install python3 on the server and sshpass on the client.
Change the ip in the inventory file

### Bootstrapping the Server
    ansible-playbook --ask-become-pass --ask-pass bootstrap.yml
Run this for:
- create an ed25519 key named ansible in your .ssh folder
- create a user on your server named robot with root permission
- copy the ed25519 key on your server

### Deploy all the stuff

    ansible-playbook run.yml

Run this for the rest

