# Dotfiles

Minimal, version‑controlled configuration files managed via **GNU Stow**.

---

## Requirements

| Package | Ubuntu install |
|---------|----------------|
| Git     | `sudo apt update && sudo apt install -y git` |
| Stow    | `sudo apt install -y stow` |
| Tree    | `sudo apt install -y tree` |

---

## Installation

```bash
# 1. Clone the repository anywhere
git clone https://github.com/CodemasterDevops421/dotfile_local.git
cd dotfile_local

# 2. Review directory layout (optional)
tree -L 2              # shows folders like bash/, zsh/, vim/

# 3. Symlink configs into $HOME
stow --target="$HOME" */   # or: stow bash zsh vim ...

