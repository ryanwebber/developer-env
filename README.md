# MacOS Developer Environment Bootstrap

Bootstraps a developer environment on MacOS.

## Getting Started

```bash
# 1. Install the xcode developer tools
xcode-select --install

# 2. Install ansible
python3 -m pip install --user ansible

# 3. Create ssh keys if needed
ssh-keygen -t ed25519 -C "$(whoami) @ $(hostname)"

# 4. Clone this repo
git clone git@github.com:ryanwebber/developer-env.git ~/.bootstrap && cd ~/.bootstrap

# 5. Run the playbook
ansible-playbook -i ./hosts.ini ./playbook.yaml
```

