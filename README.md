# Ubuntu Development Machine Workspace

This repository contains wrapper scripts and Ansible playbooks that ensures that a fresh Ubuntu Linux installation has required software and configuration to support common development environment.

This project was inspired by Jeff Geerling's [Mac Development Ansible Playbook](https://github.com/geerlingguy/mac-dev-playbook).

## Installation

Clone or download this repository into your local machine. The wrapper scripts are located in `bin/` directory. As always, before execution I encourage you to explore content of any script.

The `bootstrap` script will ensure that:

1. Existing installed packages are up to date
2. Python3.8 or above is present
3. Pip3 is present
4. Ansible is present
5. Ansible playbook `main.yml` is executed

When ready, navigate to repository root and execute the bootstrap script.

```bash
bin/bootstrap
```

Once you first ran the bootstrap script, you can use use `apply` shell script. This will skip steps 1-4 and just execute the playbook. This is useful when you want to reapply the playbook later.

```bash
bin/apply
```

## Configuration

### Default

These following UI changes will be applied:

- [Papirus Icon Theme](https://github.com/PapirusDevelopmentTeam/papirus-icon-theme)
- [Nordic theme](https://github.com/EliverLara/Nordic)
- [Yaru cursor](https://github.com/ubuntu/yaru)
- [Bind-wall](https://github.com/keshavbhatt/BingWall)

These tools and applications will be installed:

- [bat](https://github.com/sharkdp/bat)
- curl
- [gh](https://github.com/cli/cli)
- iperf
- jq
- nmap
- openssl
- [packer](https://www.packer.io/)
- shellcheck
- [terraform](https://www.terraform.io/)
- tree
- unzip
- [vagrant](https://www.vagrantup.com/)
- [vault](https://www.vaultproject.io/)
- zsh
- [brave](https://brave.com/)
- [discord](https://discord.com/)
- [postman](https://www.postman.com/)
- [spotify](https://www.spotify.com/)
- [vlc](https://www.videolan.org/vlc/)
- [code](https://code.visualstudio.com/)
- [slack](https://slack.com/)
- [virtualbox](https://www.virtualbox.org/)
- [docker](https://www.docker.com/)
- gnome-tweaks

These VScode extensions will be installed:

- [vscode-icons](https://marketplace.visualstudio.com/items?itemName=vscode-icons-team.vscode-icons)
- [material-theme](https://marketplace.visualstudio.com/items?itemName=zhuangtongfa.Material-theme)
- [ansible](https://marketplace.visualstudio.com/items?itemName=redhat.ansible)
- [vscode-yaml](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-yaml)
- [vscode-xml](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-xml)
- [trailing-spaces](https://marketplace.visualstudio.com/items?itemName=shardulm94.trailing-spaces)
- [gitlens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)
- [python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
- [vscode-pylance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance)
- [markdown-all-in-one](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)
