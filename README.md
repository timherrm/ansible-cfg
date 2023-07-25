
# Homelab Ansible Config

Ansible Configuration for my Homelab


## Ansible Server Installation

```bash
apt install pipx git sudo -y &&
pipx install --include-deps ansible &&
pipx ensurepath &&
pipx inject ansible argcomplete &&
echo 'eval "$(register-python-argcomplete pipx)"' >> /$HOME/.bashrc &&
activate-global-python-argcomplete --user &&
git clone https://github.com/timherrm/ansible-cfg &&
/root/.local/bin/ansible-galaxy install -r ansible-cfg/requirements.yml &&
ssh-keygen -f "$HOME/.ssh/id_rsa" -N "" &&
reboot
```
    
