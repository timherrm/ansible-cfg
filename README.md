
# Homelab Ansible Config

Ansible Configuration for my Homelab


## Ansible Installation

```bash
apt install pipx git -y &&
pipx install --include-deps ansible &&
pipx ensurepath &&
pipx inject ansible argcomplete &&
echo 'eval "$(register-python-argcomplete pipx)"' >> /$HOME/.bashrc &&
activate-global-python-argcomplete --user &&
git clone https://github.com/timherrm/ansible-cfg &&
ansible-galaxy install -r requirements.yml &&
ssh-keygen -f "$HOME/.ssh/id_rsa" -N "" &&
reboot
```
    
